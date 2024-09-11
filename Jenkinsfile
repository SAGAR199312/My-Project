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
    //}
//}    
       /*stage ('SonarQube analysis') {
        environment {
          scannerHome = tool 'Valaxy-SonarScanner' 
        }
            steps {
            withSonarQubeEnv('Valaxy-SonarQube-Server') 
              {
             sh '${scannerHome}/bin/sonar-scanner'
    }    
            }
        }
    }

}*/
    }
}
