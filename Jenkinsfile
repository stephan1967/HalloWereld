pipeline {
  agent any
  stages {
    stage('Joep') {
      steps {
        mail(subject: 'Hallo Maaskantjer', body: 'De groeten van Jenkins', from: 'stephan_scherders@hotmail.com', to: 'stephan_scherders@hotmail.com')
      }
    }
    stage('Anton') {
      steps {
        input(message: 'Wilt u de test starten ?', id: '100', ok: 'yes', submitter: 'no')
      }
    }
  }
}
