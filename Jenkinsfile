pipeline {
    agent any
    tools {
        jdk 'jdk8'
    }

    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven : 'maven_3_5_2') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withMaven(maven : 'maven_3_5_2') {
                    sh 'mvn test'
                }
            }
        }



    }
}
