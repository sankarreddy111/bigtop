pipeline {
    
    agent { label 'master' }
  tools {
    jdk 'Java'
    maven 'Maven'

  }

   stages {
        
        stage('Git Clone') {
            steps {
                // Get some code from a GitHub repository
                git 'https://github.com/sankarreddy111/bigtop.git'

            }

        }
        stage('Maven build') {
            steps {
                // Get some code from a GitHub repository
                sh  'mvn clean install'

            }
        }

   }
}
