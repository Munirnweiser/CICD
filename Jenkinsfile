pipeline{
    agent {

    label 'JenkinsAgent'
}
    
    tools {
        jdk 'Java17'
        maven 'Maven3'
    }
   
    stages{
        stage("Cleanup Workspace"){
            steps {
                cleanWs()
            }

        }

 
        
        stage("Checkout from SCM"){
            steps {
                git branch: 'try1', credentialsId: 'github', url: 'https://github.com/Munirnweiser/CICD.git'
            }

       

        }


}



}
