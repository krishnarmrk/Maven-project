//pipeline {
//  node('master'){
   //checkout scm
//	stages{
//	  stage ('checkout'){
//		steps {
//		checkout changelog: false, poll: false, scm: [$class: 'GitSCM', branches: [[name: 'master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'd21c2272-ffb1-459c-87cb-f4174e2d8946', url: 'https://github.com/krishnarmrk/Maven-project.git']]]
//		}
//		}
//		}
//	}
//  node('sandbox'){
//   checkout scm
//   }
// options {
//	buildDiscarder(logRotator(daysToKeepStr: '10', numToKeepStr: '5'))
//	skipDefaultCheckout(true)
//  }

//stages {
//   stage ('checkout'){
//     steps {
//      checkout changelog: false, poll: false, scm: [$class: 'GitSCM', branches: [[name: 'master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'd21c2272-ffb1-459c-87cb-f4174e2d8946', url: 'https://github.com/krishnarmrk/Maven-project.git']]]
//   }
//  }
// }
//}

pipeline {
stage "node master"
	node('master'){
		checkout scm
	}
	
stage "node sandbox"	
	node('sandbox'){
		checkout scm
	}
}