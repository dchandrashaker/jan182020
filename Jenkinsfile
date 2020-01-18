pipeline {
  agent any
  stages {
    stage('Level1') {
      steps {
        echo 'Holaaa'
      }
    }

    stage('Level2') {
      steps {
        echo 'Hola2'
      }
    }

    stage('Level3') {
      steps {
        echo 'Hola3'
      }
    }

    stage('Level4') {
      parallel {
        stage('Level4') {
          steps {
            echo 'Hola5'
          }
        }

        stage('Level3.2') {
          steps {
            echo 'stage3.2'
          }
        }

      }
    }

  }
}