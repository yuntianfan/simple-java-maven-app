pipeline {
    agent {
        docker {
            image 'maven:3-alpine' 
            args '-v /D/Users/24902/.m2:/root/.m2:z -u root'
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