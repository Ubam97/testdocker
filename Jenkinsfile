 node {
     stage('Clone repository') {
         checkout scm
     }

     stage('Build image') {
         app = docker.build("eub456/test")
     }
        stage('Push') {
            sh(script: 'docker login -u eub456 -p whrqkf12@')
            sh(script: 'docker push eub456/ruby-app:latest')
     }
}