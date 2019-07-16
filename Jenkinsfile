pipeline {
  agent any
  stages {
    stage('Stage 01') {
      parallel {
        stage('Sub-Stage 01') {
          steps {
            echo 'First step: This is sub-stage 01 in parallel'
            sleep 5
            echo 'Second step: This is sub-stage 01 in parallel'
          }
        }
        stage('Sub-Stage 02') {
          steps {
            echo 'First step: This is sub-stage 02 in parallel'
            sleep 5
            echo 'Second step: This is sub-stage 02 in parallel'
          }
        }
      }
    }
    stage('Stage 02') {
      stages {
        stage('Sub-Stage 01') {
          steps {
            echo 'First step: This is sub-stage 01 in waterfall'
            sleep 5
            echo 'Second step: This is sub-stage 01 in waterfall'
          }
        }
        stage('Sub-Stage 02') {
          steps {
            echo 'First step: This is sub-stage 02 in waterfall'
            sleep 5
            echo 'Second step: This is sub-stage 02 in waterfall'
          }
        }
      }
    }
  }
}
