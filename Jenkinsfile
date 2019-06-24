pipeline {
    agent any
    stages {

        stage('tomcat deploy'){
          steps{
		    echo 'tomcat deployment from Jenkins through Git'
                //sh 'mkdir from-jenkins'
                //sh 'touch from-jenkins/test.txt'
		    echo 'running palybook' 
                sh '''
                   ansible-playbook -i hosts tomcat.yml 
                '''
                }
        }

}
}

