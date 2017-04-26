pipeline {
    agent any

     stages {

        stage ('Build'){
           steps {
           checkout scm
           echo 'DONE'
           }
        }

        stage('Test') {
            steps {
               step([$class: 'JUnitResultArchiver', testResults: '**/target/surefire-reports/TEST-*.xml'])
            }
        }
    }
}

