pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'docker build -t ai-secure-app .'
      }
    }
    stage('Push') {
      steps {
        sh 'docker push your-dockerhub-username/ai-secure-app:latest'
      }
    }
    stage('Scan') {
      steps {
        sh 'aqua scan --image your-dockerhub-username/ai-secure-app:latest'
      }
    }
    stage('Deploy') {
      steps {
        sh 'kubectl apply -f kubernetes/ai-secure-app-deployment.yaml'
      }
    }
  }
}