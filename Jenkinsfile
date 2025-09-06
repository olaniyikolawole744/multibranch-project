pipeline {
    agent any

    stages {
        stage('Build') {
            when {
             expression{1==1}
            }
            steps {
                echo 'Building only on main branch...'
            }
        }
        stage('Deploy') {
            when {
             expression{2==2}
            }
            steps {
                echo 'Deploying only on prod branch...'
            }
        }
       stage('Monitor') {
           when {
               expression{env.BRANCH_NAME=='main'}
           }
           steps {
               echo 'Deploying on on dev branch...'
           }
         }
    }
}
