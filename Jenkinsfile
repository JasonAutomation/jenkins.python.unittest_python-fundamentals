// Powered by Infostretch 

timestamps {

node () {

	stage ('python_test1 - Checkout') {
 	 checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '', url: 'https://github.com/JasonAutomation/jenkins.python.unittest_python-fundamentals']]]) 
	}
	stage ('python_test1 - Build') {
 			// Shell build step
sh """ 
python3 -m unittest discover -s ./src/test/ -p '*_test.py' 
 """ 
	}
}
}
