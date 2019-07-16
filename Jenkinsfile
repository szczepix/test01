pipeline {
  agent any
  stages {
    stage('Stage 01') {
      parallel {
        stage('Sub-Stage 01') {
          steps {
            echo 'This is sub-stage 01 in parallel'
          }
        }
        stage('Sub-Stage 02') {
          steps {
            echo 'This is sub-stage 02 in parallel'
          }
        }
      }
    }
    stage('Stage 02') {
      stages {
        stage('Sub-Stage 01') {
          steps {
            echo 'This is sub-stage 01 in parallel'
          }
        }
        stage('Sub-Stage 02') {
          steps {
            echo 'This is sub-stage 02 in parallel'
          }
        }
      }
    }
  }
}
