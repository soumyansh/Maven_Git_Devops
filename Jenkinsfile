pipeline {
    agent any
    

stages{
        stage('Init'){
            steps {
                echo 'Starting..'
            }
           
        }

        stage ('Building'){
           
                   steps {
                echo 'Building ..'
				bat 'mvn clean package'
            }
			post{
			success{
			echo 'Now Archiving'
			archiveArtifacts artifacts: '**/target/*.war'
			}
			}
           
        }

                stage ("Deploy to Production"){
                    steps {
                        echo 'Code deployed..'
                    }
                }
            }
        }
    