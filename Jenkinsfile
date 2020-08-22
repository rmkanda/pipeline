pipeline {
  agent {
    kubernetes {
      yamlFile 'build-agent.yaml'
      defaultContainer 'docker-cmds'
      idleMinutes 1
    }
  }
  stages {
    stage('Setup') {
      parallel {
        stage('Install Dependencies') {
          steps {
            container('docker-cmds') {
              sh 'ls'
            }
          }
        }
        stage('Secrets scanner') {
          steps {
            container('docker-cmds') {
              sh 'ls'
            }
          }
        }
      }
    }
    stage('Build') {
      steps {
        container('docker-cmds') {
          sh 'ls'
        }
      }
    }
    stage('Unit Tests') {
      steps {
        container('docker-cmds') {
          sh 'ls'
        }
      }
    }
    stage('Package') {
      steps {
        container('docker-cmds') {
          sh 'ls'
        }
      }
    }
    stage('Deploy') {
      steps {
        // TODO
        sh "echo done"
      }
    }
  }
}
