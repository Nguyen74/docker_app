node{
    stage("Git clone"){   
       	git credentials: 'GIT_HUB_CREDENTIALS', url: 'https://github.com/Nguyen74/docker_app.git'   
    }
    stage("Docker build"){
	sh 'whoami'
	sh 'sudo docker build -t nbpn123/nnguyen:v1 .'
	sh 'sudo docker image'
    }   
     
    withCredentials([string(credentialsId: 'DOCKER_HUB_PASSWORD', variable: 'PASSWORD')]){   
        sh 'sudo docker login -u nbpn123 -p 0848877500n'   
    }   
      
}
