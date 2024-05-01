pipeline{
    
    agent any 
    
    stages {
        
        stage('Git Checkout'){
            
            steps{                    
                    git branch: 'main', url: 'https://github.com/nitin-mukesh/demo-counter-app.git'
                }
            }
         stage('integration testing'){
            
            steps{  
                    sh 'mvn verify -DskipUnitTests'
                }
            }
        
    }
}
