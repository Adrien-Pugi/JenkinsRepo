pipeline {
   
	agent any
   
    stages {

        stage('get code from github+gitHook') {
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