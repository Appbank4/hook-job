pipeline{
	agent any
	stages{
		stage('1-RepoClone'){
			steps{
				sh 'df-h'
			}
		}
		stage('2-CPUAnalysis'){
			steps{
				sh 'lscpu'
			}
		}
		stage('3-memoryCheck'){
			steps{
				sh 'gree-g'
			}
		}
        stage('OSAnalysis'){
            steps{
                sh 'cat /etc/os-release'
            }
        }
	}
}