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
                        error 'index.html n\'existe pas'
                    }
                }
            }
        }
    }
}


/* CORRECTION
pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        echo 'Démarrage du build...'
      }
    }
    stage('Test') {
      steps {
        script {
          echo 'Démarrage des tests...'
          if (fileExists('index.html')) {
            echo "Fichier index.html présent"
          } else {
            error "Fichier index.html manquant"
          }
        }
      }
    }
  }

  post {
    success { echo 'OK ✅' }
    failure { echo 'Échec ❌' }
  }
}
*/
