node{

stage 'checkout'
   git url: 'https://github.com/claudiadelriego/Example-Pipeline.git'

stage 'Build'
   echo 'DONE'

stage 'Build2'
sh 'make check || true'
sh step([$class: 'JUnitResultArchiver', testResults: '**/target/surefire-reports/TEST-*.xml'])

}
