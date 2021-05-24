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
          steps {
            sh 'ci/build-app.sh'
          }
        }

      }
    }

  }
}