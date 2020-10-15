pipeline {
    agent any
    stages {
        stage('Test') {
		steps {
               		bat 'set'
            	      }
        }
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
    post {
        always {
            echo 'This will always run'
        }
        success {
            echo 'This will run only if successful'
        }
        failure {
            echo 'This will run only if failed'
        }
        unstable {
            echo 'This will run only if the run was marked as unstable'
        }
        changed {
            echo 'This will run only if the state of the Pipeline has changed'
            echo 'For example, if the Pipeline was previously failing but is now successful'
        }
    }
}
