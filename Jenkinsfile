pipeline {
    agent any

    tools {
       
        maven "maven3.8.4"
    }

    stages {
        stage('Build') {
            steps {
                
               git credentialsId: '787bae0c-80a9-4fd1-82d7-ddaecd084b2a', url: 'https://github.com/mss-ec-appsdecbatch/maven-web-application.git'

                sh "mvn clean package"

            }

        }
    }
}
