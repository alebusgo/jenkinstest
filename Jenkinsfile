pipeline {

    agent any
<<<<<<< HEAD

=======
    
       
>>>>>>> 14497e332e91f7a7f168ed48aff94d61f3e27189
    stages {
        stage('Executing Gradle') {
            steps {
<<<<<<< HEAD
                echo 'Building the application ...'
                withGradle() {
                    sh 'gradlew clean build -x test'
=======
                echo 'Executing gladle ...'
                withGradle(){
                    sh './gradlew -v'
>>>>>>> 14497e332e91f7a7f168ed48aff94d61f3e27189
                }
            }
        }
        
        stage("Build") {
             steps {
                echo 'Building the application ...'
                sh 'gradle clean build -x test '
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









