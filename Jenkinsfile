@Library('my-shared-lib@main') _

pipeline {
  agent any
  stages {
    stage('Use shared hello') {
      steps {
        echo "Calling shared library function hello(...)"
        hello('Guru')                    // from shared-lib vars/hello.groovy
      }
    }
    stage('Call shared pipeline (demo)') {
      steps {
        echo "Demo finished"
      }
    }
  }
}