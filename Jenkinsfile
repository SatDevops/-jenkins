pipeline {
    agent any 
    environment{
        ENV_URL= "Pilpline.google URL"
          SSH_CRED = credentials('SSH-Cenos7')
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
               sh "env"
            }
        }
    }

}