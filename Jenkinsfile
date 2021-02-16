pipeline {
  agent any
  stages {
    stage('hello world') {
      steps {
        echo 'hola mundo!'
        sh 'echo %PATH%'
      }
    }

    stage('crear archivo') {
      steps {
        writeFile(file: 'prueba.txt', text: 'contenido del archivo')
      }
    }

  }
}