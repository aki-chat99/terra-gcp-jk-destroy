pipeline {
  agent any
  stages {
    stage('Destroy infra') {
      steps {
        echo 'destroying infra'
        ws(dir: '/var/lib/jenkins/demo1') {
          sh '''cd /var/lib/jenkins/demo1
pwd
sh iac_gcp_destroy.sh
'''
        }
        
      }
    }
  }
}