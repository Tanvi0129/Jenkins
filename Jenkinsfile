node{
    stage('git clone'){
      git credentialsId: 'pt', url: 'https://github.com/Tanvi0129/Jenkins.git'
     }
    stage('maven clean'){
	   sh 'maven clean'
	 }
    stage('maven Validate') {
	   sh 'maven Validate'
     }
	stage('maven Compile') {
	   sh 'maven Compile'
	 }
	stage('maven Test') {
	   sh 'maven Test'  
	 }
	stage('maven Deploy'){
	   sh 'maven Deploy'
	 }
	stage('maven Package'){
	   sh  'maven Package'
	 }
	}
