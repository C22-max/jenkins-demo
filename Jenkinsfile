pipeline {
    agent any
    tools {
        nodejs 'node'
    }
    stages {
        stage('check version') {
            steps {
                sh'node --version'
            }
        }

        stage('Clone repo') {
            steps {
                git(
            url:"https://github.com/C22-max/jenkins-demo.git",
            branch:"master"
        )
            }
        }
        stage('Installnpm') {
            steps {
                sh'npminstall'
            }
        }

        stage('Tests') {
            steps {
                echo "Running tests"
                }
        }
    stage('Run app locally'){
        steps{
            sh 'nohup node index.js &'
        }
}
  
              
           }
       }

