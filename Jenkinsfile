pipeline {
  agent any
  stages {
    stage('git') {
      steps {
        git(url: 'https://github.com/divyanshu-srivastava/demo-repo.git', branch: 'test', poll: true)
      }
    }
    stage('') {
      steps {
        sshPublisher(masterNodeName: 'test')
      }
    }
  }
}