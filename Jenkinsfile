pipeline {
    agent { label 'nodejs' }
   
    stages{
        stage ('sourcecode'){
            steps {
                git branch: 'declarative', url: 'https://github.com/ramyapatibandla48/js-e2e-express-server.git'
            }

        }
        stage(' shellcommands') {
            steps {
                sh '''npm install
                    npm run build
                    npm pack
                    '''
            }
        }
    }

    
}
