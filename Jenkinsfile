node{

stage 'checkout'
   git url: 'https://github.com/claudiadelriego/Example-Pipeline.git'

stage 'Build'
   echo 'DONE'

stage 'Build2'
sh step([$class: 'SampleTest', testResults: '**/target/surefire-reports/TEST-*.xml'])

}
