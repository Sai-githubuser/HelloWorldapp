pipeline (
  agent any 
  stages {
     stage ('Git-Checkout') {
       steps {
        git url: 'https://github.com/Sai-githubuser/HelloWorldapp.git'
         echo "Checkout Successful";
      }
    }
    
    stage ('Compile) {
      steps {
       bat label: '', script: 'mvnw compile'
        echo "test successful";
      }
    }
    
    stage ('Build') {
     steps {
        bat label: '', script: 'mvnw clean'
        bat label: '', script: 'mvnw package'
        echo "build successful";
       }
    }
          
      stage ('Test') {
          steps{
            bat label: '', script: 'mvnw test'
            echo "test successful";
          }
       }
    }
  }
               

  

  
        
