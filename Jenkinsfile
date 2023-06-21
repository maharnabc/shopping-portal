pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
   tools{
       nodejs  'nodejs' 
    }
 

    stages{
        stage('build-the-job'){
            steps{
                echo 'this is the build the app job'
                sh 'npm install'
            }
        }
        stage('test'){
            steps{
                echo 'this is the test the app job'
                sh 'npm test'
            }
        }
        stage('package'){
            steps{
                echo 'this is the packege the app job'
                sh 'npm run package'
            }
        }
    }
    
    post{
        always{
            echo 'Hello there.. My 1st pipeline..completed.'
        }
        
    }
    
}
