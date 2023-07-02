pipeline{
	agent any
	stages{
		stage('1-RepoClone'){
			steps{
				checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'git-Id', url: 'https://github.com/Appbank4/hook-job.git']])
			}
		}
		stage('2-CPUAnalysis'){
			steps{
				sh 'lscpu'
			}
		}
		stage('3-memoryCheck'){
			steps{
				sh 'free -g'
			}
		}
        stage('OSAnalysis'){
            steps{
                sh 'cat /etc/os-release'
            }
        }
        stage('5-WelcomeMessage'){
            steps{
                echo "Welcome To Cyberlord"
            }
        }
	}
}