pipeline {
  agent any
  stages {
    stage('Stage 01') {
      parallel {
        stage('Stage 01') {
          steps {
            echo 'This is stage 01'
          }
        }
        stage('Stage 02') {
          steps {
            echo 'This is stage 02'
          }
        }
      }
    }
    stage('Stage 03') {
      steps {
        echo 'Stage 03'
      }
    }
  }
}