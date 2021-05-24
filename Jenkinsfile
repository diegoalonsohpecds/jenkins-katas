pipeline {
  agent any
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
              image 'gradle:6.8.3-jdk11'
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