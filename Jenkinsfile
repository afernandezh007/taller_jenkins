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

  }
  environment {
    minombre = 'Antonio'
  }
}