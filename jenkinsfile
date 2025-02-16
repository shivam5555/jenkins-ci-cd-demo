pipeline {
    agent any  // Run on any Jenkins agent

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/shivam5555/jenkins-ci-cd-demo.git'
            }
        }

        stage('Build') {
            steps {
                sh 'echo "Building the application..."'
                sh 'sleep 2'
            }
        }

        stage('Test') {
            steps {
                sh 'echo "Running tests..."'
                sh 'sleep 2'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo "Deploying application..."'
                sh 'sleep 2'
                sh 'cp index.html /var/www/html/'  // Simulated deployment
            }
        }
    }
}

