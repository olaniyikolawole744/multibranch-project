pipeline {
    agent any

    stages {
        stage('Build') {
            when {
             expression{${env.BRANCH_NAME}=='main'}
            }
            steps {
                echo 'Building only on main branch...'
            }
        }
        stage('Deploy') {
            when {
             expression{${env.BRANCH_NAME}=='prod'}
            }
            steps {
                echo 'Deploying only on prod branch...'
            }
        }
       stage('Monitor') {
           when {
               expression{${env.BRANCH_NAME}=='dev'}
           }
           steps {
               echo 'Deploying on on dev branch...'
           }
         }
    }
}
