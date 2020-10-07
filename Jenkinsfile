pipeline {
  agent {
    kubernetes {
      yamlFile 'build-agent.yaml'
      defaultContainer 'docker-cmds'
      idleMinutes 1
    }
  }
  stages {
    stage('Install Dependencies') {
      steps {
        container('docker-cmds') {
          sh 'ls'
        }
      }
    }
    stage('Build Application') {
      steps {
        container('docker-cmds') {
          sh 'ls'
        }
      }
    }
    stage('Unit Test') {
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
    stage('Publish') {
      steps {
        container('docker-cmds') {
          sh 'ls'
        }
      }
    }
    stage('Deploy to TEST env') {
      steps {
        // TODO
        sh "echo done"
      }
    }
    stage('Deploy to PROD env') {
      steps {
        // TODO
        sh "echo done"
      }
    }
  }
}
