 node {
     stage('Clone repository') {
         checkout scm
     }

     stage('Build image') {
         app = docker.build("eub456/test")
     }
     stage ('Push Image'){
         docker.withRegistry('https://registry.hub.docker.com', 'test')
         app.push("${env.BUILD_NUMBER}")
         app.push("latest")
     }
}