pipeline {
agent {node {label ''}}
   
//	properties([buildDiscarder(logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '10', numToKeepStr: '10')), parameters([string(defaultValue: 'ramakrishna', description: '', name: 'myname', trim: false)])])

  options {
	buildDiscarder(logRotator(daysToKeepStr: '10', numToKeepStr: '5'))
	skipDefaultCheckout(true)

  }
stages {
   stage ('checkout'){
     steps {
      checkout changelog: false, poll: false, scm: [$class: 'GitSCM', branches: [[name: 'master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'd21c2272-ffb1-459c-87cb-f4174e2d8946', url: 'https://github.com/krishnarmrk/Maven-project.git']]]
   }
  }
 }


}
