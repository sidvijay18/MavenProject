node {
	//def server = Artifactory.server 'artifactory' 
    //def rtMaven = Artifactory.newMavenBuild()
    //def buildInfo
    //def mvnHome
   // jdk = tool name: 'JAVA8'
   // env.JAVA_HOME = "${jdk}"
    
   stage ('Code Checkout') {			
	git branch: 'master', url: "https://github.com/ChiragMakkar13/MavenProject.git"
		}
	
	stage('Unit Testing') {
      junit '**/target/surefire-reports/TEST-*.xml'
   }	
	stage (' Code Build') {
	    sh 'mvn package'
    }
   
	//stage('SonarQube analysis') {
        //mvnHome = tool 'mavenhome'
	//	withSonarQubeEnv('sonar') {
        //rtMaven.run pom: 'pom.xml', goals: '$SONAR_MAVEN_GOAL -Dsonar.host.url=$SONAR_HOST_URL', buildInfo: buildInfo
	//	}
//	}
	
 
	
	//stage('Docker Image Build'){
	  // sh "sudo docker build -t chiragmakkar13/mavendemo:Dockerfile ."
          //}

    //stage('Push Image') {
      //      withCredentials([usernamePassword(
        //    credentialsId: "dockerhub",
          //  usernameVariable: "USER",
            //passwordVariable: "PASS"
        //)]) {
          //  sh "sudo docker login -u $USER -p $PASS"
        //}

        //sh "sudo docker tag chiragmakkar13/mavendemo:latest chiragmakkar13/mavendemo:$BUILD_NUMBER"
        //sh "sudo docker push chiragmakkar13/mavendemo:latest"
        //sh "sudo docker push chiragmakkar13/mavendemo:$BUILD_NUMBER"
    //} 
	
	
	
 }







