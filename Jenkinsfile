pipeline{
    agent any
    stages{
        stage("SCM Checkout"){
            steps{
                git 'https://github.com/sea-region/my-app'
            }
        }
        stage("Compile Package"){
            steps{
                sh 'mvn -q clean package'
            }
        }
   
    }
}
