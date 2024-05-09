pipeline {

    agent any

    stages {

        stage('Build') {

            steps {

                groovy Build

            }

        }

        stage('Test') {

            steps {

                sh 'echo "Testing..."'

                sh 'pwd'

                sh 'touch testfile.txt'

                sh 'ls -l'

            }

        }

        stage('Deploy') {

            steps {

                sh 'touch ./deploy.sh'

                sh 'cat ./deploy.sh'

                sh 'echo "Deploying..."'

                sh 'mv testfile.txt /tmp'

                sh 'ls -l /tmp'

            }

        }

    }

}
