pipeline{
  agent any
  parameters{
    booleanParam(name: 'DeployPod', defaultValue: true)
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
  post {
      success{
        echo "Your job is success ......."
      }
      failure{
        echo "your job is fail ......."
      }
      always{
        echo "always go ahead ...."
      }
    }
   
}









