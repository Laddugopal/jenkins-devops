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
	stages {
		stage('Build') {
			steps {
				echo "Hare Krishna"
			}
		}
		stage('Test') {
			steps {
				echo "Chant and be Happy"
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
