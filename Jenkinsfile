pipeline {
    agent any
    stages {
        stage ('Compile Stage'){
            steps{
                bat 'python get-pip.py'
                bat 'pip install -r requirements.txt'
                bat 'run.py'
                
            }
        }
        stage ("Test Stage"){
            steps{
                bat 'python test.py'
            }
        }
    }
}