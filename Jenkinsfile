pipeline{
	agent { docker {image 'maven:3.9.5'}}
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