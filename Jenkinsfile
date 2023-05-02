pipeline { 
    
  agent any 
       
      stages{  
            stage('Remove old container') { 
               steps { 
                   sh 'docker rm -f nodejs_app'
                  //    sh 'echo remove old container'
               }
            }
            stage('Build docker container') { 
                steps { 
                     sh 'docker build -t todo-node-app .'
                 }
            }
          stage('Run docker container') { 
                 steps { 
                     sh 'docker run -itd --name nodejs_app -p 8000:8000 todo-node-app'
                 }
             }
        }
 }
