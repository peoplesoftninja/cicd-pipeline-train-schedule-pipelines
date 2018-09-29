pipeline{
  agent any
    stages{
      stage('Build'){
        steps {
        echo 'Building The Project train-schedule'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
      }
    }
}
