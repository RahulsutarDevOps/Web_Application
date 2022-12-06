pipeline {
    agent any 
    stages {
        stage('httpd') { 
          steps {
            sh 'sudo yum install httpd -y' 
              }
        }
        stage('start') {
            steps {
            sh 'sudo systemctl start httpd'
            }
        }
        stage('create') {
            steps {
            sh 'echo "Hi Rahul How Are You" >> index.html'
            sh 'cp -r index.html /var/www/html'
            sh 'chmod 777 /var/www/html/index.html'
          }  
        }
    }
}
