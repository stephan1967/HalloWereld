pipeline {
    agent any
    stages {
        stage('Show settings') {
		steps {
               		bat 'set'
            	      }
        }
	stage('Send mail') {
		steps {
        		mail(subject: 'Hallo Maaskantje', body: 'De groeten van Jenkins', from: 'stephan_scherders@hotmail.com', to: 'stephan_scherders@hotmail.com')
      		      }
        }
	stage('Show dialog') {
      		steps {
        		input(message: 'Wilt u de test starten ?', id: '100', ok: 'Ja', submitter: 'Nee')
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
            echo 'This will run only if the state of the Pipeline has changed. eg if the Pipeline was previously failing but is now successful'
        }
    }
}
