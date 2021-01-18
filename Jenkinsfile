pipeline {
    agent none

    stages {

        stage ('Hello') {
            agent any

            steps {
                echo 'Hello, '
		echo 'this houldtrigger a build '
                echo 'yet another change'
		sh '''#!/bin/bash

                    echo "Hello from bash"
                    echo "Who I'm $SHELL"
		    /usr/local/bin/aws --version
                '''
            }
        }
    }
}


