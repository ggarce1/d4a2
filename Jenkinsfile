pipeline{
checkout scm	
agent any
	stages{
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
