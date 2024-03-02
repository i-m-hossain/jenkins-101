pipeline{
    agent{
        node{
            label 'docker-agent-alpine'
        }
    }
    triggers{
        pollSCM 'H/5 * * * *'
    }
    stages{
        stage('Build'){
            steps{
                echo "Building..."
                sh '''
                echo "doing build stuff..."
                '''
            }
        }
        stage('Test'){
            steps{
                echo "testing..."
                sh '''
                echo "doing test stuff"
                '''
            }
        }
        stage('Deliver'){
            steps{
                echo "deliver..."
                sh '''
                echo "doing delivery stuff"
                '''
            }
        }
    }
}