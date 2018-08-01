pipeline {
  agent any
  stages {
    stage('clean stage') {
      steps {
       withMaven(maven: 'maven') {
         sh 'mvn clean'
	}
	}
	}
    stage('compile stage') {
      steps {
        withMaven(maven: 'maven') {
          sh 'mvn compile'
	}
	}
	}
    stage('test stage') {
      steps {
        withMaven(maven: 'maven') {
          sh 'mvn test'
	}
	}
	}
    stage('package stage') {
      steps {
        withMaven(maven: 'maven') {
            sh 'mvn package'
	}
	}	
	}
	stage('install stage') {
          steps {
            withMaven(maven: 'maven') {
            sh 'mvn install'
        }
        }
        }
}
}
 

