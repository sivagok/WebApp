pipeline {
  agent any
  stages {
    stage('Dev Code Pull') {
      steps {
        echo 'Dev Coe pull done'
      }
    }

    stage('Dev Maven Build') {
      steps {
        echo 'Dev Maven Build Done'
      }
    }

    stage('Deploy to QA ') {
      steps {
        echo 'QA Deploy Done'
      }
    }

    stage('UI Test') {
      parallel {
        stage('UI Test') {
          steps {
            echo 'UI Code Pull done'
            echo 'UI Test done'
          }
        }

        stage('API Test') {
          steps {
            echo 'API Code Pull Done'
            echo 'API test done'
          }
        }

      }
    }

    stage('Certify QA') {
      steps {
        echo 'QA certified'
      }
    }

    stage('UAT Deploy') {
      steps {
        echo 'UAT Deploy done'
      }
    }

    stage('UAT Certify') {
      steps {
        echo 'UAT Certified'
      }
    }

    stage('Prod Deploy') {
      steps {
        echo 'Prod Deploy Done'
      }
    }

  }
}