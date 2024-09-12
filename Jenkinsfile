pipeline{
    agent {
        node { 
           label "maven-agent"
        }
    }
    environment {
        PATH = "/opt/apache-maven-3.9.9/bin:$PATH"
    }
    stages {
        stage ('build') {
            steps {
                sh 'mvn clean deploy'
           
             }
        }
    }
}    
       /*stage ('SonarQube analysis') {
        environment {
          scannerHome = tool 'SonarQube-Scanner' 
        }
            steps {
            withSonarQubeEnv('SonarQube-Server') 
              {
             sh '${scannerHome}/bin/sonar-scanner'
    }    
            }
        }
    }

}*/
    
