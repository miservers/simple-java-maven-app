pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                withMaven(
                   // maven installation declared in "Global Tool Configuration"
                   maven: maven-2
                ){
                   sh 'mvn -B -DskipTests clean package'
                 } 
            }
        }
    }
}
