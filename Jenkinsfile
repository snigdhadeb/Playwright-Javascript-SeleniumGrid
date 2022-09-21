pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        bat 'npx playwright test'
      }
      post {
        always {
            archiveArtifacts artifacts: 'playwright-report/*'
            //below artifacts will only be stored, if trace, video and screenshots are 'on' and build is
            //successful at least for one time, so for the first time, its recommended to 
            //turn on video/trace/screenshots in the config file and then comment out the next two lines and build it.
            //for the next run uncomment the two lines
            archiveArtifacts artifacts: 'playwright-report/data/*'
            archiveArtifacts artifacts: 'test-results/*/*.zip'
        }
      }
    }
  }
}
