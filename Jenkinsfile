pipeline {
  agent any {
  stages {
    stage ('build') {
      steps {
        echo 'Running Gradle'
        sh './gradlew build no-demon'
        archiveArtifacts artifacts: '/dist/trainSchedule.zip'
        }
      }
    }
}
