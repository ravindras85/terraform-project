pipeline {
 agent any
 
 stages {
   stage(‘checkout’) {
   	steps {
	git url: ‘https://github.com/ravindras85/terraform-project.git’
       }
      }

   stage(‘Set Terraform path’) {
	steps {
	script {
	def tfHome = tool name: ‘Terraform’
	env.PATH = “${tfHome}:${env.PATH}”
 	}
	sh ‘terraform -version’
	}
       }
 
