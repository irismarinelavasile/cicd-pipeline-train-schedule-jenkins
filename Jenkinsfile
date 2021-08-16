pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArctifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
