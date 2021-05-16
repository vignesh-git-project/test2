pipeline {
    agent any

    stages {
        stage ('Composer Install') {

            steps {
                 {
                    sh 'composer install'
                    
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                 {
                    sh 'npm install'
                }
            }
        }


        stage ('Install Stage') {
            steps {
                 {
                    sh 'npm run dev'
                }
            }
        }
    }
}
