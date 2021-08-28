 node {
     stage('Clone repository') {
         checkout scm
     }

     stage('Build image') {
         app = docker.build("test/image")
     }
     stage ('Push Image'){
         docker.withRegistry('https://hub.docker.com/repository/docker/eub456/test', 'test')
     }
}