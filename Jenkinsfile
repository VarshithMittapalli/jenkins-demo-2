pipeline{
    agent any

    stages{
        stage('checkout code'){
            steps{
                echo 'Featching code from git hub'
                checkout scm
            }
        }
        stage('Run python script'){
            steps{
                echo 'Runnig python script'
                sh 'python3 hello.py'
            }
        }
    }

    post {
        success{
            echo 'build is success......'
        }
        failure{
            echo 'build is failure'
        }
    }
}