#!groovy 



node {

   stage 'Checkout'

        checkout scm



   stage 'Setup'

        sh 'npm install --python=python2.7'



   stage 'Mocha test'

        sh './node_modules/mocha/bin/mocha'



   stage 'Cleanup'

        echo 'prune and cleanup'

        sh 'npm prune'

        sh 'rm node_modules -rf'

}
