pipeline{
	agent any
		tools{
			maven 'Maven 3.6.3'
		}
	stages{
			stage('build'){
				steps{
					echo 'compiling sysfoo app'
					sh 'mvn compile'
				}
			}

			stage('test'){
				steps{
					echo 'unit test sysfoo app'
					sh 'mvn clean test'
				}
			}

			stage('package'){
				steps{
					echo 'packaging sysfoo app'
					sh 'mvn package -DskipTests'
				}
			}
	}
}