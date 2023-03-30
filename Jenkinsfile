node{
    stage("Git clone"){   
       	git credentials: 'GIT_HUB_CREDENTIALS', url: 'https://github.com/Nguyen74/docker_app.git'   
    }
    stage("Docker build"){
	sh 'whoami'
	sh 'docker build -t nbpn123/nnguyen:v1 .'
	sh 'docker image'
    }   
     
    withCredentials([string(credentialsId: 'DOCKER_HUB_PASSWORD', variable: 'PASSWORD')]){   
        sh 'docker login -u nbpn123 -p 0848877500n'   
    }   
      
}
