pipeline {
  agent {
    docker {
      image 'gradle:jdk11'
    }

  }
  stages {
    stage('Say Helloweeee') {
      parallel {
        stage('Say Helloweeee') {
          steps {
            sh 'echo "hello world"'
          }
        }

        stage('Build App') {
          agent {
            docker {
              image 'gradle:jdk11'
            }

          }
          steps {
            sh 'ci/build-app.sh'
          }
        }

      }
    }

  }
}