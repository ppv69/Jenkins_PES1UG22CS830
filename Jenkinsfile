pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ PES1UG22CS830_Task_5.cpp -o temp'
                 build job: 'PES1UG22CS830-1', wait: false
                 echo 'Build Successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat PES1UG22CS830_Task_5.cpp'
                echo 'Test Successful'
            }
        }

        stage('Deploy') {
            steps {
               
                 echo 'Deploy Successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
