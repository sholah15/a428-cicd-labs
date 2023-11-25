node {
    // Define the Docker agent with the desired image and arguments
    docker.image('node:16-buster-slim').withRun('-p 3000:3000') {
        
        // Stage: Build
        stage('Build') {
            // Steps for the Build stage
            sh 'npm install'
        }
        
        // Stage: Test
        stage('Test') {
            // Steps for the Test stage
            sh './jenkins/scripts/test.sh'
        }
        
        // You can add more stages as needed
    }
}
