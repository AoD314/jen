pipeline {
  agent any
  
  stages {
    stage("test stage #1") {
      steps {
        echo "test message #1"
        echo "test message #2"
      }
    }
    stage("test stage #2") {
      steps {
        script {
          echo "test message #1"
          echo "test message #2" >> log.txt
          echo "$PATH"
          bash "python -version"
        }
      }
    }
  }
}
