pipeline {
    agent any


    environment {
        BUILDDIR = "${HOME}/backdemo/"
        PROJECT_NAME = "gs-test-demo"
    }

    stages {

        stage ("Init Config") {
            steps {
                script {
                    env
                }
            }
        }
        stage('代码 Clone') {
            steps {
                sh "cd /root/backdemo/gs-test-demo;sudo mvn test; sudo mvn clean;"

            }
        }


    }
}
