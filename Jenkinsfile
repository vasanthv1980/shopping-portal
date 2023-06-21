pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
   tools{
       nodejs 'nodejs' 
    }
    

    stages{
        stage('build-the-app'){
            steps{
                echo 'this is to build the app'
                sh 'npm install'
            }
        }
        stage('test-the-app'){
            steps{
                echo 'this is to test the app job'
                sh 'npm test'
            }
        }
        stage('package-the-app'){
            steps{
                echo 'this is package the app'
                sh 'npm run package'
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}
