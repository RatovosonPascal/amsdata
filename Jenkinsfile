pipeline {
   
    agent any
   
    stages {

        stage('get code from github') {
            steps {
                echo 'Pulling...';
                git branch: 'master',
                url : 'git@github.com:RatovosonPascal/amsdata.git';
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