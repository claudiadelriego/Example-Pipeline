pipeline {
    agent any

     git url: 'https://github.com/claudiadelriego/Example-Pipeline.git', branch: 'master'

     stages {

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

