// pipeline {
//     agent any

//     parameters {
//         string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')

//         text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')

//         booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')

//         choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')

//         password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
//     } 
//     environment{
//         ENV_URL= "Pilpline.google URL"
//        // SSH_CRED = credentials('SSH-Cenos7')
//     }
//      tools {
//         maven 'maven-3.8.6' 
//     }
   
//      stages {
       
//     //   stage('stage two' ) {
//     //     steps {
//     //            sh  "echo ENV_URL= ${ENV_URL}"
//     //            sh "mvn --version"
         
//     //         }
//     //     }
//     stage('two' ) {
//         when { environment name: 'CHOICE', value: 'One' }
//         steps {
//                    sh "echo This Stage is executed as this Choice is ONE"
//             }
//         }

//     //   stage('Two' ) {
//     //     input {
//     //             message "Should we continue?"
//     //             ok "Yes, we should."
//     //             submitter "alice,bob"
//     //             parameters {
//     //                 string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
//     //             }
//     //           }
//     //     steps {
//     //             echo "Hello, ${PERSON}, nice to meet you."
         
//     //         }
//     //     }
//     }

// }



pipeline {
   agent { label 'java' } 
   // agent any
    stages {
        stage('Parallel Stages') {
            parallel {
            stage('One') {
                steps {
                    sh "sleep 3"
                    sh "curl ifconfig.co"
                }
            }
            stage('Two') {
                steps {
                    sh "sleep 4"
                }
            }
            stage('Three') {
                steps {
                    sh "sleep 5"
                }
            }
        }
    }
        stage('Four') {
            steps {
                sh "sleep 1"
            }
        }
        stage('Sowmya') {
            steps {
                sh "sleep 1"
            }
        }
    }

}