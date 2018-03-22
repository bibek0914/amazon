pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven : 'MAVEN_HOME') {
                    bat cd 'com.Amazon & mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withMaven(maven : 'MAVEN_HOME') {
                    bat cd 'com.Amazon & mvn test'
                }
            }
        }


        stage ('Deployment Stage') {
            steps {
                withMaven(maven : 'MAVEN_HOME') {
                    bat cd 'com.Amazon & mvn deploy'
                }
            }
        }
    }
}
