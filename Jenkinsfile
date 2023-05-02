pipeline { 
    
  agent any 
       
      stages{  
            stage('Remove old container') { 
               steps { 
                   sh 'docker rm -f nodejs_app'
                    // sh 'echo remove old container'
               }
            }
            stage('Build docker image') { 
                steps { 
                     sh 'docker build -t todo-node-app .'
                 }
            }
          // stage('Docker Login'){
            
           // steps {
             //    withCredentials([string(credentialsId: 'Dockerid', variable: 'Dockerpwd')]) {
               //     sh "docker login -u sutarrahul -p ${Dockerpwd}"
           //     }
         //   }                
     //   }
        // stage('Docker Push'){
           // steps {
             //   sh 'docker push sutarrahul/springboot:12.2.0-alpine'
          //  }
      //  }
          stage('Run docker container') { 
                 steps { 
                     sh 'docker run -itd --name nodejs_app -p 8000:8000 todo-node-app'
                 }
             }
        }
 }
