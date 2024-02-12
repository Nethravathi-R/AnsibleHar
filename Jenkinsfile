pipeline {
  agent any
  
  stages {
    stage('checkout stage') {
      steps {
        sh 'rm -rf AnsibleHar'
        sh 'git clone https://github.com/Nethravathi-R/AnsibleHar.git'
      }
    }
    stage('running playbook') {
      steps {
        sh 'ansible-playbook -i hosts grafana.yml'
      }
    }
  }
}
