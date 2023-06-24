pipeline {
  agent any
  
  stages {
    stage('scan') {
      steps {
        // Perform build steps (e.g., installing dependencies) for your Python application
        sh 'Hello World'
        // sh 'pip install Flask'
      }
    }
    
    stage('Deploy') {
      steps {
        // Perform deployment steps for your Python application
        //sh 'pm2 delete python-api'
        //sh 'pm2 delete python-web-project'
        //sh 'pm2 start "python3 app.py" --name python-web-project'
        sh 'Hello world'
      }
    }
  }
}
