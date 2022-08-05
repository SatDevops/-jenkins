pipeline {
    agent any 
    environment{
        ENV_URL= "Pilpline.google URL"
    }

    stages {
        stage('stage one' ) {
            steps {
                echo 'heloo task one'
            }
        }

        stage('stage two' ) {
            steps {
               sh  "echo ENV_URL= ${ENV_URL}"
            }
        }
    }

}