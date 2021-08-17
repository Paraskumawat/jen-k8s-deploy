pipeline{
  agent any
  stages{
    stage('Deploy'){
      steps{
        sh " kubectl apply -f deploy.yml --kubeconfig /admin.conf"
      }
    }
  } 
}









