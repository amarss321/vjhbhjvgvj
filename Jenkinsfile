pipeline {
    agent any

    stages {
        stage('countinous download') {
            steps {
                git 'https://github.com/boxfuse/boxfuse-sample-java-war-hello.git'
            }
        }
        stage('countinous build') {
            steps {
                sh 'mvn install'
            }
        }
        stage('countinous deployment') {
            steps {
                sh 'cp target/hello-1.0.war /opt/apache-tomcat-9.0.60/webapps' 
            }
        }
    }
}

