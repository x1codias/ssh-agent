node {
  stage('do something with git') {  
    sshagent (credentials: ['github-key']) {
      // get the last commit id from a repository you own
      sh 'git ls-remote -h --refs git@github.com:x1codias/ssh-agent.git master |awk "{print $1}"'
    }
  }
}