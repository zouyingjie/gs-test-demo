pipeline {
    agent any
    
    tools {
        maven 'M3'
    }

    environment {
        BUILDDIR = "${HOME}/backdemo/"
        PROJECT_NAME = "gs-test-demo"
        

    }

    stages {

        stage ("Init Config") {
            steps {
                script {
                    sh "env"
                }
            }
        }
        stage('代码 Clone') {
            steps {
                sh "cd /root/backdemo/gs-test-demo; mvn test;  mvn clean;"

            }
        }


    }
}
