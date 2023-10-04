pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                script {
                    if (env.BRANCH_NAME == 'main') {
                        echo 'Hello from main branch'
                    }  else {
                        sh "echo 'Hello from ${env.BRANCH_NAME} branch!'"
                    }
                    }
            }
        }
    }
}

stage('Gmail')
{
	steps
	{
		emailext body: "*${currentBuild.currentResult}:* Job Name: 
                ${env.JOB_NAME} || Build Number: ${env.BUILD_NUMBER}\n More 
                information at: ${env.BUILD_URL}",
		subject: 'Jenkin Taskis',
		to: 'shygul10@gmail.com'
	}
}

