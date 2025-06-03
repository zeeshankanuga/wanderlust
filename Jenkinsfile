pipeline {
    agent any

    environment {
        SONAR_HOME = tool "sonar"
    }

    stages {
        stage('Clone Repository') {
            steps {
                git url: "https://github.com/zeeshankanuga/wanderlust.git", branch: "main"
            }
        }

        stage('SonarQube Quality analysis') {
            steps {
                withSonarQubeEnv('sonar') {
                    sh "$SONAR_HOME/bin/sonar-scanner -Dsonar.projectKey=wanderlust -Dsonar.projectName=wanderlust"
                }
            }
        }

        stage('OWASP Dependency check') {
            steps {
                dependencyCheck additionalArguments: '--scan ./', odcInstallation: 'dc'
				dependencyCheckPublisher pattern: '**/dependency-check-report.xml'
            }
        }

        stage('Trivy File system Scan') {
            steps {
                sh "trivy fs --format table --output trivy-fs-report.xml ."
            }
        }
        stage('Deploy using Docker Compose') {
            steps {
                sh 'docker-compose down'
                sh 'docker-compose up -d --force-recreate'
            }
        }
    }
}
