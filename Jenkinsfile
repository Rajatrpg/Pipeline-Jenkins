pipeline{
    agent any

    stages{
        stage("compile"){
            steps{
                sh 'javac Test.java'
            }
        }
        stage("run"){
            steps{
                sh 'java Test'
            }
        }
    }

    post{
        always{
            sh 'echo "always"'
        }
        sucess{
            sh 'echo "success"'
        }
        failure{
            sh 'echo "faliure"'
        }
    }
}