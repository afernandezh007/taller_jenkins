pipeline {
  agent any
  stages {
    stage('crear archivo') {
      steps {
        writeFile(file: 'prueba.txt', text: 'contenido del archivo')
        archiveArtifacts '*.txt'
      }
    }

    stage('helloworld') {
      steps {
        bat 'SET'
        echo 'Hello world'
        bat 'echo %minombre%'
      }
    }

    stage('despedida') {
      steps {
        input(message: 'lastima que termino!!', ok: 'Excelente taller!!')
      }
    }

  }
  environment {
    minombre = 'Antonio'
  }
}