pipeline{
  agent any
  parasmeters{
    booleanParam(name: 'DeployPod', defaultValue: 'true')
  }
  stages{
    stage('Deploy'){
      when{
        expression{
          params.DeployPod
        }
      }
      steps{
        sh " kubectl apply -f deploy.yml --kubeconfig /admin.conf"
      }
    }
  } 
}









