pipeline{	
agent any
	stages{
		 stage('Clone repository') {
        /* Let's make sure we have the repository cloned to our workspace */

        checkout scm
   		 }
		stage('Initial Setup'){
			steps{
				sh 'echo Starting..' 
			}
		}
		stage('Checking Docker'){
			steps{
				sh 'sudo docker ps'
			}
		}
		stage('Build Docker'){
			steps{
				sh 'sudo docker build -t nuevaImagen:v1 .'
			}
		}
	}
}
