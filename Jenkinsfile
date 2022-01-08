node{
    stage('git clone'){
      git credentialsId: 'git', url: 'https://github.com/Tanvi0129/Jenkinsfile.git'
     }
    stage('maven clean'){
         sh 'mvn clean'
    }
    stage('maven Validate'){
         sh 'mvn Validate'
    }
    stage('maven Compile'){
	 sh 'mvn Compile' 
    }
    stage('maven Test'){
	 sh 'mvn Test'  
    }
    stage('maven Deploy'){
	 sh 'mvn Deploy'
    }
    stage('maven Package'){
	 sh  'mvn Package'
    }
}
