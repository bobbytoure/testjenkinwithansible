node {
  stage('do something with git') {  
    // sshagent (credentials: ['idtoto']) {
    withCredentials([sshUserPrivateKey(credentialsId: "idtoto", keyFileVariable: 'keyfile')]) { 
     // test ansible command
      sh 'ls'
      sh 'ansible --version'
      sh 'ssh -i ${keyfile} -tt -o StrictHostKeyChecking=no toto@157.230.106.21'
    }
  }
}

