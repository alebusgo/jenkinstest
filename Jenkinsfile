pipeline {

    agent any
    tools {
        gradle '7.4.2'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building the application ...'
                sh 'gradle clean build -x test'
            }
        }

        stage("test1") {
             steps {
                echo 'excecuting automated test1'
                sh 'gradle clean test aggregate'

             }
        }

        stage("test2") {
            steps {
                echo 'excecuting automated test2'
                sh 'gradle clean test -Denvironment=qa aggregate'

            }
        }

        stage("test3") {
            steps {
                echo 'excecuting automated test3'
                sh 'gradle clean test -Denvironment=prov aggregate'

            }

        }


    }
}









