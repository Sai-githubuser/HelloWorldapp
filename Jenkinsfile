pipeline (
  agent any 
  stages {
     stage ('Git-Checkout') {
       steps {
        git url: 'https://github.com/Sai-githubuser/HelloWorldapp/new/master'
         echo "Checkout Successful";
      }
    }
    
    stage ('Compile) {
      steps {
       bat label: '', script: 'mvn compile'
        echo "test successful";
      }
    }
    
    stage ('Build') {
     steps {
        bat label: '', script: 'mvn clean'
        bat label: '', script: 'mvn package'
        echo "build successful";
       }
    }
          
      stage ('Test') {
          steps{
            bat label: '', script: 'mvn test'
            echo "test successful";
          }
       }
    }
  }
               

  

  
        
