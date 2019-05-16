pipeline {
agent {node {label ''}}
   
	properties([buildDiscarder(logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '10', numToKeepStr: '10')), parameters([string(defaultValue: 'ramakrishna', description: '', name: 'myname', trim: false)])])

}
