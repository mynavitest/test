pipeline{
    agent any
    stages{
        stage('Server Details'){
            steps{
                echo 'Server Details'
                sh 'uname -a'
            }
        }
        stage('Date'){
            steps{
                sh 'DATE'
            }
        }
        stage('cpu usage'){
            steps{
                sh 'free -hf'
            }
        }
    }
}
