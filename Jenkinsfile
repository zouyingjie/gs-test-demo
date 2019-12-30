pipeline {
    agent any


    environment {
        BUILDDIR = "${HOME}/backdemo/"
        PROJECT_NAME = "gs-test-demo"
        MAVEN_HOME="/usr/local/apache-maven-3.6.2"
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
