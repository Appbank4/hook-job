pipeline{
	agent any
	stages{
		stage('1-make a left'){
			steps{
				sh 'action-1'
			}
		}
		stage('2-make a right'){
			steps{
				sh 'action-2'
			}
		}
		stage('3-make a left'){
			steps{
				sh 'action-3'
				sh 'action-4'
			}
		}
	}
}