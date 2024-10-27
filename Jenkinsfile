pipeline{
    agent any
    stages{
        stage('Clonando repo'){
            steps{
                git branch: 'main',
                    url: 'https://github.com/DianaLlamoca/Pruebas.git'
            }
        }
        stage('Instalando dependencias'){
            steps{
                //Realizo la instalación de las dependencias localizadas en el package.json
                sh "npm install"
            }
        }
        stage('Iniciando la aplicación en el puerto 3000'){
            steps{
                sh "node index.js"
            }
        }
    }
}
