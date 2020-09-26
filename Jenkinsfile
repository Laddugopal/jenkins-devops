//SCRPITED
//node {
//	stage('Build') {
//		echo "Build"
//	}
//	stage('Test') {
//		echo "Test"
//	}
//	stage('Preprod Test') {
//		echo "Preprod Test"
//	}
//}
//DECLARATIVE
pipeline{
	agent any
	environment {
		mavenHome = tool 'Laddumaven'
		PATH ="mavenHome/bin:$PATH"
	}
	stages {
		stage('Checkout') {
			steps {
				sh 'mvn --version'
				echo "Hare Krishna"
			}
		}
		stage('Compile') {
			steps {
				sh "mvn clean compile"
			}
		}
		stage ('Test') {
			steps {
				sh "mvn test"
			}
		}
	}
	post {
		always {
			echo "Hare Krishna Hare Ram"
		}
		success {
			echo "Hare Krishna Hare Ram Mahamantra"
		}
		failure {
			echo " Do chanting daily"
		}
	}
}
