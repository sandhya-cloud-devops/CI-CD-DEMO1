pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Starting CI build...'
                echo 'Checking application files...'
                sh 'ls -la'
                sh 'test -f index.html'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Starting deployment...'
                sh 'sudo /usr/bin/cp index.html /var/www/html/index.html'
                echo 'Deployment completed successfully!'
            }
        }
    }
}
