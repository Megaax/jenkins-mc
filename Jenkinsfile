pipeline{
	agent { docker {image 'maven:3.6.3'}}
	stages{
		stage('Build'){
			steps{
				sh 'mvn --version'
				echo "build"
			}
		}
		stage('Test'){
			steps{
				echo "Test"
			}
		}
		stage('IntegerationTest'){
			steps{
				echo "IntegerationTest"
			}
		}
	}
	post{
		success{
			echo 'stages successful'
		}
		failure{
			echo 'stages failed'
		}
	}
}