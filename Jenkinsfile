node{
    stage("Git clone"){   
       	git credentials: 'GIT_HUB_CREDENTIALS', url: 'https://github.com/Nguyen74/docker_app.git'   
    }
    stage("Docker build"){
	sh 'whoami'
	sh 'sudo docker build -t nbpn123/nnguyen:v1 .'
	sh 'sudo docker image'
    }   
     
      
}
