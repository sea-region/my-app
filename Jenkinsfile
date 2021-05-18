pipeline{
    agent any
    tools{
     maven 'maven3'   
    }
    stages{
        stage("SCM Checkout"){
           steps{
                git 'https://github.com/sea-region/my-app'
            }
        }
        stage("Compile Package"){
            steps{
                def mavehome = tool name: 'maven3', type: 'maven'
                sh "mvn -q clean package"
            }
        }
   
    }
}
