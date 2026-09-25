node {
    stage('Checkout') {
        checkout scm
    }

    stage('Run Application') {
        bat '"C:\\Users\\mugdh\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" app.py'
    }

    stage('Build Docker Image') {
        bat 'docker build -t devops-practical-3 .'
    }

    stage('Run Docker Container') {
        bat 'docker run --rm devops-practical-3'
    }

    echo 'CI/CD Pipeline completed successfully!'
}