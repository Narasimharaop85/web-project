pipeline {
    agent any
    stages {
        stage ('Initialize') {
            steps {
                sh '''
                    cd /var/lib/jenkins/javaproject
                    git clone https://github.com/Narasimharaop85/web-project.git 
                    echo ${git}
                    echo ${maven}
                    echo "M2_HOME = ${MAVEN_HOME}"
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
