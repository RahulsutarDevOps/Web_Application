pipeline {
    agent any

    stages {
        stage('httpd') {
            steps {
                sh "sudo yum install httpd -y"
                sh "sudo service httpd start"
            }
        }
        
    }
}
