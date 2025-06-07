pipeline{
    agent any

    stages{
        stage('checkout code'){
            step{
                echo 'Featching code from git hub'
                checkout scm
            }
        }
        stage('Run python script'){
            step{
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