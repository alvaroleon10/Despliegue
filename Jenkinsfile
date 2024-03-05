pipeline {
    agent any
    
    
    tools {
        maven 'Maven'
    }

    
    stages {
        stage('Clonar Repositorio') {
            steps {
               git branch: 'master', url: 'https://github.com/alvarojimeenez/calculadoraSpring.git'
            }
        }
        
        stage('Construir Aplicación') {
            steps {
                 
                    sh 'mvn clean package -DskipTests=true'
                 
            }
        }

    }
}
