pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Construccion de artifact 2.0'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'       
      }
    }
  }
}
