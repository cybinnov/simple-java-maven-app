pipeline {
    agent {
        docker {
            image 'maven:3.8.5-adoptopenjdk-11' 
            args '-v /root/.m2:/root/.m2'
	    args '/Users/tkondasani' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
