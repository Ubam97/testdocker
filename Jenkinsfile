 node {
     stage('Clone repository') {
         checkout scm
     }

     stage('Build image') {
         app = docker.build("eub456/test")
     }
        stage('Push') {
            sh(script: 'docker login -u eub456 -p ????')
            sh(script: 'docker push eub456/test:latest')
     }
}
