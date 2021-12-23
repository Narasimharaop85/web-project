pipeline {
    agent any
    stages {
        stage ('Initialize') {
            steps {
                sh '''
                    cd /var/lib/jenkins/javaproject
                    git clone https://github.com/Narasimharaop85/web-project.git 
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                '''
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('codequality') {
            steps {
                echo 'quality gate passed....'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
