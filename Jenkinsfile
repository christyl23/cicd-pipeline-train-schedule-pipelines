pipeline {
  agent any
  stages {
    steps {'Build'} {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveartifacts 'dist/trainSchedules.zip'
      }
    }
  }
}
