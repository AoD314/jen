pipeline {
  agent any
  
  stages {
    stage('test stage #1') {
      steps {
        echo 'test message #1'
        echo 'test message #2'
      }
    }
    stage('Parallel In Sequential') {
      parallel {
        stage('In Parallel 1') {
          steps {
            echo "In Parallel 1"
          }
        }
        stage('In Parallel 2') {
          steps {
            echo "In Parallel 2"
          }
        }
      }
    }    
    stage('test stage #2') {
      steps {
        echo 'test message #1'
        echo '$PATH'
        sh 'ls'
        sh 'echo "test message #2" >> log.txt'
        sh 'python -version'
      }
    }
  }
}
