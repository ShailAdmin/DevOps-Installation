DevOps Tools Installation
 
	Git
	Maven
	Jenkins
	Docker
	Kubernetics
	Ansible
	Teraform
	Grafana
	ELK
	
Git Installation : -

         Step-1 Create AWS Machine
	 Step-2 yum install git
	 step-3 git --version
		 
Maven Installation : -

         Step-1 Create AWS machine
	 step-2 yum install maven
	 Step-3 maven --version
		 
Jenkins Installation : -

		 Step-1 Creat AWS Machine
		 Step-2 
		  
		      wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat-stable/jenkins.repo
                      rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key
		      yum upgrade
                      yum install jenkins java-1.8.0-openjdk-devel -y
                      systemctl daemon-reload
		      systemctl enable jenkins
		      systemctl start jenkins
		      systemctl status jenkins
		 Step-3 rpm -qa | grep jenkins
		 
Docker Installation : -

         Step-1 Create AWS Machine
	 Step-2 Docker installation 
		 
		       
	        yum install -y yum-utils
		yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
		yum-config-manager --enable docker-ce-nightly
		yum-config-manager --enable docker-ce-test
		yum install docker-ce docker-ce-cli containerd.io -y
	 Step-3 docker --version
		 
Kubernetics Installation : -

         Step-1 Creat AWS Machine
	 Step-2 Kubernetic installation
		     Kubctl installation: -
			 
		      curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
	              curl -LO "https://dl.k8s.io/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl.sha256"
                      echo "$(<kubectl.sha256) kubectl" | sha256sum --check
                      install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl
		      kubectl version --client
		 kop Installation : -
		  curl -LO https://github.com/kubernetes/kops/releases/download/$(curl -s https://api.github.com/repos/kubernetes/kops/releases/latest | grep tag_name | cut -d '"' -f 4)/kops-linux-amd64
		  chmod +x kops-linux-amd64
		  mv kops-linux-amd64 /usr/local/bin/kops
		  kops version
			  
Ansible Installation : -

         Step-1 Create AWS Machine
	 Step-2 
	 
	      upgrade python to python38
	      pip38 install ansible
	      ansibel --version
			  
Teraform Installation : -

         Step-1 Create AWS Machine
	 step-2 
	        yum install -y yum-utils
		yum-config-manager --add-repo https://rpm.releases.hashicorp.com/RHEL/hashicorp.repo
		yum -y install terraform
	 Step-3	terraform --version
				
Grafana Installation : -

         Step-1 yum list grafana
                yum install grafana
         Step-2 systemctl daemon-reload
                systemctl enable grafana-server
                systemctl start grafana-server
                systemctl status grafana-server
	 Step-3 rpm -qa | grep Grafana
			
		 
