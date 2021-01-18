pipeline {
    agent none

    stages {

        stage ('Hello') {
            agent any

            steps {
                echo 'Hello, '
		echo 'this houldtrigger a build '
		echo 'test polling'
		echo 'this should trigger now'
		sh '''#!/bin/bash

                    echo "Hello from bash"
                    echo "Who I'm $SHELL"
		    /usr/local/bin/aws --version
                '''
            }
        }
    }
}


