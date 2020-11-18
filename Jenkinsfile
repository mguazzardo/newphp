pipeline {

  agent any

  stages {

    stage('Build') {


      steps {

        script {

          openshift.withCluster() {

	    openshift.newApp( 'https://github.com/mguazzardo/hello-php' ).narrow('bc')
          }

        }

      }

    }

  }

}
