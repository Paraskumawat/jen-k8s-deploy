pipeline{
  agent any
  stages{
    stage('Deploy'){
      steps{
        sh " kubectl get pod --kubeconfig admin.conf"
      }
    }
  } 
}









