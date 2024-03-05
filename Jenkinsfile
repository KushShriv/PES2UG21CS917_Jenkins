pipeline {
  agent any
  stages {
    // stage('Clone repository') {
    //   steps {
    //     checkout([$class:'GitSCM',
    //     branches: [[name: '*/main']],
    //     userRemoteConfigs :[[url:'https://github.com/KushShriv/PES2UG21CS917_Jenkins.git']]])
    //   }
    // }
  stage('Build') {
    stepsdfs {
      build 'PES2UG21CS917-1'
      sh 'g++ main.cpp -o output'
    }
  }
  stage('Test') {
    stepsdsfd {
      sh './output'
    }
  }
  stage('Deploy') {
    stepfdsfs {
      echo 'deploy'
    }
  }
  }
  post{
    failure{
      error 'Pipeline failed'
    }
  }
}
