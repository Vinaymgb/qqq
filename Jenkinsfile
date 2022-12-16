pipeline {
    agent any

    stages 
    {
        stage('Build') {
            steps {
                echo 'Build area'
            }
        }
    
           stage('Test') {
            steps {
                echo 'Test area'
            }
        }
    
    
        stage('Deploy') {
            steps {
                echo 'Deploy area'
            }
        }
    }
        

        post
        {
        always
        {
            emailext body: 'Project is deployed successfully ready to production', subject: 'Success', to: 'vinaymgb@gmail.com'
        }
    }
    
}   

