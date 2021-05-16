pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven : 'maven_3_5_0') {
                    sh 'mvn clean compile -s mvn-settings.xml'
                    
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withMaven(maven : 'maven_3_5_0') {
                    sh 'mvn test -s mvn-settings.xml'
                }
            }
        }


        stage ('Install Stage') {
            steps {
                withMaven(maven : 'maven_3_5_0') {
                    sh 'mvn install -s mvn-settings.xml'
                }
            }
        }
    }
}
