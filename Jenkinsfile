pipeline {
   
	agent any
   
    stages {

        stage('get code from github') {
            steps {
                echo 'Pulling...';
                git branch: 'master',
                url : 'https://github.com/Adrien-Pugi/JenkinsRepo';
            }

            post {
                success {
                    echo "====++++success++++===="
                }
               
                failure {
                    echo "====++++failed++++===="
                }
            }
           
        }
           
    }
}