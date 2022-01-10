// Declrative pipeline
pipeline{
	agent any
	stages{
		stage('Build'){
			steps{
				echo "Build"
			}
		}

		stage('Test'){
			steps{
				echo "Test"
			}
		}

		stage('Integration Test'){
			steps{
				echo "Integration Test"
			}
		}
	}

	post{
		always{
			echo "All ok!"
		}
		success{
			echo "All steps ran successfully"
		}
		failure{
			echo "Some stage is failed"
		}
		changed{
			echo "The status has changed"
		}
	}
}