pipeline{
  agent any
    stages{
      stage('Build'){
        steps {
        echo 'Building The Project train-schedule'
        sh './gradlew build --no-daemon'
        sh './gradlew npm_start'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
      }
    }
}
