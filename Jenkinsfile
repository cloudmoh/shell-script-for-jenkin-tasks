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

