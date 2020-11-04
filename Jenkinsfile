pipeline {
    agent any
    stages {
        stage ('Checkout') {
          steps {
            git 'https://github.com/Arvind3534/spring-petclinic-1.git'
          }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
                junit '**/target/surefire-reports/*.xml'
            }
        }
    }
}
