node{
    stage('git clone'){
      git credentialsId: 'git', url:'https://github.com/Tanvi0129/pt.git'
     }
    stage('maven clean'){
         sh 'mvn clean'
     }     
    stage('maven Validate'){
         sh 'mvn validate'
    }
    stage('maven Compile'){
	 sh 'mvn compile' 
    }
    stage('maven Test'){
	 sh 'mvn test'  
    }
    stage('maven Deploy'){
	 sh 'mvn deploy'
    }
    stage('maven Package'){
	 sh  'mvn package'
    }
    stage('maven Install'){
	 sh  'mvn install'
    }
    stage('maven Pre-Clean'){
	 sh 'mvn pre-clean'
    }
}
