 node {
     stage('Clone repository') {
         checkout scm
     }

     stage('Build image') {
         app = docker.build("eub456/test")
     }
<<<<<<< HEAD
        stage('Push') {
            docker.withRegistry('https://registry.hub.docker.com', 'jenkinsfordockerhub') {
                sh(script: 'docker push eub456/test:latest')
        }
=======
        stage('Push image') {
            sh(script: 'docker login -u eub456 -p ????')
            sh(script: 'docker push eub456/test:latest')
>>>>>>> 7c6e3242558ac048210eea98c31a994dda1c6d9f
     }
}
