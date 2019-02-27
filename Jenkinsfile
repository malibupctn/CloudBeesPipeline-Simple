pipeline {
  agent any
  stages {
    stage('hello') {
      steps {
        sleep 5
        echo 'hello PCTN'
      }
    }
    stage('goodbye') {
      parallel {
        stage('goodbye') {
          steps {
            echo 'bye'
          }
        }
        stage('parallel step') {
          steps {
            sleep 2
            echo 'parallel step'
          }
        }
      }
    }
  }
}