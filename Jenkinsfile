def foo = "foo"
pipeline {
 agent any
 
 stages {
   stage('checkout') {
   	steps {
	git url: 'https://github.com/ravindras85/terraform-project.git'
       }
      }

 stage ('for testing')
        sh "echo ${foo}"
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
