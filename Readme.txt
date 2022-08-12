  1.  Docker image  of  springboot application is created via docker file.
  
  
  2. Need to have aws ECR repo. to push the image into repo.
     aws ecr get-login-password --region eu-central-1 | docker login --username AWS --password-stdin 378612673110.dkr.ecr.eu-central-1.amazonaws.com/java-demo
	 
	 
  3. tag the docker image with repo name and push to ECR
     docker tag image_name:latest ECR repo url
	 
	 docker push ECR Url:latest
	 
	 
  4.  	 terraform init
         terraform validate
		 terraform plan
		 terraform apply
     
  
  
  