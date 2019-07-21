node {
  stage('do something with git') {  
    sshagent (credentials: ['idtoto']) {
      // test ansible command
      sh 'ansible --version'
    }
  }
}
