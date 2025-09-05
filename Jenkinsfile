pipeline {
    agent any

    stages {
        stage('Build') {
            when {
                branch 'main'
            }
            steps {
                echo 'Building only on main branch...'
            }
        }
        stage('Deploy') {
            when {
                branch 'prod'
            }
            steps {
                echo 'Deploying only on prod branch...'
            }
        }
       stage('Monitor') {
           when {
               branch 'dev'
           }
           steps {
               echo 'Deploying on on dev branch...'
           }
         }
    }
}
