pipeline{
	agent any
// -- Descarga código desde SCM
   echo 'Descargando código de SCM'
   sh 'rm -rf *'
   checkout scm
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
`		stage('Build Docker'){
			steps{
				sh 'sudo docker build -t nuevaImagen:v1 .'
			}
		}
	}
}
