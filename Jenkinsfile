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
                sh '$date'
            }
        }
        stage('cpu usage'){
            steps{
                sh 'ps -eo pid,user,%cpu,comm --sort=-%cpu | head -10'
            }
        }
        stage('memory usage'){
            steps{
                sh 'free -h'
            }
        }
        stage('disk usage'){
            steps{
                sh 'df -h'
            }
        }   
    }
}