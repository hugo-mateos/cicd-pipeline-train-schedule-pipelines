pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
    //stage ('Deploy') {
      // steps {
      //  echo 'Ejecutando el deploy'
      //}
    //}
  }
}
