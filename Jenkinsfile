pipeline {
  agent {
    docker { image 'gaahrdner/packer-ansible-resource:latest' }
  }
  stages {
    stage('Test') {
      steps {
        sh 'packer init .'
        sh 'packer build aws-ami-v1.pkr.hcl
      }
    }
  }
}