pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo '🚧 1. BUILD: Compilando código...'
                echo '✅ Build completado.'
            }
        }
        stage('Test') {
            steps {
                echo '🧪 2. TEST: Ejecutando pruebas unitarias...'
                echo 'Prueba 1: OK'
                echo 'Prueba 2: OK'
                echo '✅ Todas las pruebas pasaron.'
            }
        }
        stage('Deploy') {
            steps {
                echo '🚀 3. DEPLOY: Desplegando aplicación...'
                echo '✅ Aplicación desplegada en entorno de prueba.'
            }
        }
    }
    
    post {
        success {
            echo '🎉 PIPELINE EXITOSO!'
        }
        failure {
            echo '💥 PIPELINE FALLIDO.'
        }
    }
}
