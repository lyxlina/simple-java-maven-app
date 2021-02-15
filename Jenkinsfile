pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('GetCode') {
      steps {
        sleep 5
      }
    }
    stage('build') {
      steps {
        sh '/var/local/apache-maven-3.6.3/bin/mvn clean install -DskipTests'
      }
    }
  }
}
