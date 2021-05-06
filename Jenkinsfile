pipeline {
    agent any
    
    environment {
        DEMO = '1'
    }
    
    stages {
        stage('Hello') {
            steps {
                echo "This is build number $BUILD_NUMBER of demo $DEMO"
                sh '''
                    echo "Usinng external script"
                    chmod +x  test.sh
                '''
            }
        }
    }
}