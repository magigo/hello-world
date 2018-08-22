pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '''#!/bin/bash
DOCKER_LOGIN=`aws ecr get-login --region cn-north-1`
${DOCKER_LOGIN}'''
      }
    }
  }
}