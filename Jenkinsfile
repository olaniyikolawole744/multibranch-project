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
                echo  "THIS IS DEV BRANCH"
                echo "THIS IS ENV DOT GIT BRANCH: ${env.GIT_BRANCH}"
                echo "THIS IS BRANCH URL ${env.GIT_URL}"
                echo "THIS IS PRINT ENV ${printenv}"
            }
        }
       stage('Monitor') {
           when {
               expression{6==6}
           }
           steps {
               echo "THIS IS BRANCH NAME: ${BRANCH_NAME}"
           }
         }
    }
}
