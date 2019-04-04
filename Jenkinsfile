pipeline {
 agent any
 
 stages {
   stage('checkout') {
   	steps {
	git url: 'https://github.com/ravindras85/terraform-project.git'
       }
      }

   stage('Verify Terraform') {
	steps {
//	def tfHome = tool name: 'terraform', type: 'org.jenkinsci.plugins.terraform.TerraformInstallation'
//	env.PATH = "${tfHome}"
	  sh "/usr/local/bin/terraform -version"
	}
     } 
}
}
