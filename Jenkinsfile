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
                echo 'Package Job ..'
				build job: 'Package '
            }
		
           
        }

                stage ("Deploy to stage"){
                    steps {
                        echo 'deploying to stage..'
                        
                    }
                }
            }
        }
    