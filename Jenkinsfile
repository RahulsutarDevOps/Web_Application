pipeline {
    agent any 
    stages {
        stage('httpd') { 
          steps {
            sh 'yum install httpd -y' 
              }
        }
        stage('start') {
            steps {
            sh'service httpd start'
            }
        }
        stage('create') {
            steps {
            sh 'touch index.html'
            sh 'echo "Hi Rahul How Are You" >> index.html'
            sh 'cp -r index.html /var/www/html'
            sh 'chmod 777 /var/www/html/index.html'
          }  
        }
    }
