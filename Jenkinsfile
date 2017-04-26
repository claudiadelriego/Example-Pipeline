pipeline {
    agent any
stages {
 stage ('checkout') {
     git url: 'https://github.com/claudiadelriego/Example-Pipeline.git'
}


        stage ('Build'){
           steps {

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

