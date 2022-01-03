node {
    stage('Git Clone') { 
	  git credentialsId: 'git', url: 'https://github.com/kartikeyapro/ks.git'
    }
    stage('Maven Clean') {
        sh 'mvn clean'
    }
    stage('Maven Validate') {
        sh 'mvn validate'
    }
	stage('Maven Validate') {
		sh 'mvn sonar:sonar -Dsonar.host.url=http://34.68.2.232:9000 -Dsonar.login=c03b084c29bdf53c6a033069a53c5616802692b8'
	}
	 stage('Maven Compile') {
        sh 'mvn compile'
    }
	 stage('Maven Test') {
        sh 'mvn test'
    }
	 stage('Maven Package') {
        sh 'mvn package'
    }
	 stage('Maven Deploy') {
        sh 'mvn deploy'
    }
}

