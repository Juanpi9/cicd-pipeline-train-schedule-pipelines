pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Construccion de artifact'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
              
      }
    }
  }
}
