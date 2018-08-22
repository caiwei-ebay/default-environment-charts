pipeline {
  options {
    disableConcurrentBuilds()
  }
  agent {
    label "raptor-tess-builder"
  }
  environment {
    DEPLOY_NAMESPACE = "change-me"
  }
  stages {
    stage('Validate Environment') {
     steps {
          sh "echo Environment Validated! Good to deploy!
        }
    }
    stage('Update Environment') {
      when {
        branch 'master'
      }
      steps {
          sh "echo Your application deployed/applied via Helm sucessfully!
        }
    }
  }
}
