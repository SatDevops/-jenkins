pipeline {
    agent any

    parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')

        text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')

        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')

        choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')

        password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
    } 
    environment{
        ENV_URL= "Pilpline.google URL"
       // SSH_CRED = credentials('SSH-Cenos7')
    }
     tools {
        maven 'maven-3.8.6' 
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