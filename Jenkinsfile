pipeline {
  agent any
  
  stages {
    stage('Build') {
      steps {
        // Perform build steps (e.g., installing dependencies) for your Python application
        sh 'ls'
        sh 'pip install Flask'
        
      }docker run -itd -p "1234:1234" python-web:latest  
    }
    
    stage('Deploy') {
      steps {
        // Perform deployment steps for your Python application
        sh 'pm2 delete python-api'
        sh 'pm2 start "python3 app.py" --name python-api'
      }
    }
  }
}
