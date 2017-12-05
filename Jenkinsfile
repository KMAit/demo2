pipeline {
	agent any
	
	stages {
		stage('Build') {
			steps {
				bat 'mvn -B -DskipTests clean package'
				bat 'mvn test'
				bat 'dir /S target'
			}
		}
	}
}