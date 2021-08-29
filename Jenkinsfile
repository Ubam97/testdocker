 node {
     stage('Clone repository') {
         checkout scm
     }

     stage('Build image') {
         app = docker.build("eub456/test")
     }

     stage('Push image') {
            docker.withRegistry('https://registry.hub.docker.com', 'test') {
                sh(script: 'docker push eub456/test:latest')
            }
        }
 }
    
