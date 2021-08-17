pipeline{
  agent any
  stages{
    stage('Deploy'){
      when{
        expression{
          false
        }
      }
      steps{
        sh " kubectl apply -f deploy.yml --kubeconfig /admin.conf"
      }
    }
  } 
}









