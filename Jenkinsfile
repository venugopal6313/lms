pipeline {
    agent any

    stages {
        stage('Sonar Analysis') {
            steps {
                echo 'CODE QUALITY CHECK'
                // Below command works in jenkins 
                sh 'cd webapp && sudo docker run --rm -e SONAR_HOST_URL="http://172.212.227.13:9000" -v ".:/usr/src" -e SONAR_TOKEN="sqp_7482310ee178c2c3a4be5b12aab21148954411b6" sonarsource/sonar-scanner-cli -Dsonar.projectKey=lms'
                echo 'CODE QUALITY COMPLETED'    
            }
        }
        
    }
}