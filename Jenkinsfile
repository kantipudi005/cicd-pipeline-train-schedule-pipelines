pipeline {
  agent any
  stages {
    stage ('build') {
      steps {
        echo 'Running automation'
        sh './gradlew build --no-daemon'
        archieveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
