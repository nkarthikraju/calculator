pipeline {
  agent any
  stages {
    stage('Stage1') {
      parallel {
        stage('Stage1') {
          steps {
            sleep(time: 1, unit: 'SECONDS')
            echo 'hello world'
          }
        }
        stage('Stage2') {
          steps {
            echo 'hellio'
          }
        }
      }
    }
    stage('stage2.1') {
      parallel {
        stage('stage2.1') {
          steps {
            echo 'hi'
            echo 'hjk'
          }
        }
        stage('stage2.2') {
          steps {
            sleep(time: 1, unit: 'MINUTES')
          }
        }
      }
    }
    stage('temp') {
      steps {
        build 'job2'
      }
    }
    stage('temp') {
      steps {
        build 'job1'
      }
    }
  }
}