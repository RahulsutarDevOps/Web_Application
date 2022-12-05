pipeline {
    agent any 
            stages {
        stage('FIRST-STAGE') { 
          steps {
            sh 'sudo yum install httpd -y' 
              }
        }
        stage('SEC-STAGE') {
            steps {
            sh'sudo service httpd start'
            }
        }
        stage('THI-STAGE') {
            steps {
            sh 'sudo touch index.html'
            sh 'echo "Hi Rahul How Are You" >> index.html'
            sh 'sudo cp -r index.html /var/www/html'
            sh 'sudo chmod 777 /var/www/html/index.html'
          }  
        }
    }
}

