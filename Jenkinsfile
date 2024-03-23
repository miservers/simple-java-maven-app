pipeline {
    agent any
    tools {
      // maven installation declared in "Global Tool Configuration"
      maven 'maven-3.8.7'
    }
    stages {
        stage('Build') { 
            steps {
                 sh 'mvn -B -DskipTests clean package'
            }
        }
        stage('Deploy') {
            steps {
                 print 'Hello Jenkins'
            }
        }
    }
}
