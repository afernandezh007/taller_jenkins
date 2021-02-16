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
        bat 'echo %PATH%'
      }
    }

  }
  environment {
    minombre = 'Antonio'
  }
}