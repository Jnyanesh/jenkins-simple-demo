pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git url: 'https://github.com/Jnyanesh/jenkins-simple-demo.git',
                    branch: 'main'
            }
        }

        stage('Run Script') {
            steps {
                sh 'chmod +x script.sh'
                sh './script.sh'
            }
        }
        stage('Run python file'){
            steps{
                sh python3 simple.py
            }
        }

    }
}
