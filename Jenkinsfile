pipeline {
  agent any
  stages {
    stage('Joep') {
      steps {
        mail(subject: 'hallo allemaal', body: 'njnvkvndjvndfjkvnkjdfnvkdfn', from: 'stephan_scherders@hotmail.com', to: 'stephan_scherders@hotmail.com')
      }
    }
    stage('Anton') {
      steps {
        input(message: 'Wilt u de test starten ?', id: '100', ok: 'yes', submitter: 'no')
      }
  }
}
