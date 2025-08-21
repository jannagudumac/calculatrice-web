pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Début du build'
            }
        }
        stage('Test') {
            steps {
                script {
                    if (fileExists('index.html')) {
                        echo 'index.html existe'
                    } else {
                        echo 'index.html n\'existe pas'
                    }
                }
            }
        }
    }
}
