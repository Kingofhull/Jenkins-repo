pipeline {
    agent any
    tools {
        maven "Maven3"
        jdk "OracleJDK8"
    }


    environment {
<<<<<<< HEAD
        SNAP_REPO = "vprofile-snapshot"
        NEXUS_USER = "admin"
        NEXUS_PASS = "admin"
        RELEASE_REPO = "vprofile-release"
	    CENTRAL_REPO = "vpro-maven-central"
        NEXUSIP = "172.31.13.76"
=======
        SNAP_REPO = 'vprofile-snapshot'
        NEXUS_USER = 'admin'
        NEXUS_PASS = 'password'
        RELEASE_REPO = 'vprofile-release'
	CENTRAL_REPO = 'vpro-maven-central'
        NEXUSIP = 'IP'
>>>>>>> 2360a9eea58c5c9265679ade9561c647818789c6
        NEXUSPORT = '8081'
        NEXUS_GRP_REPO = 'vpro-maven-group'
        NEXUS_LOGIN = 'nexuslogin'
      
    }

    stages {
        stage('Build'){
            steps {
                sh 'mvn -s settings.xml -DskipTests install'
            }
        }
    }
<<<<<<< HEAD
=======

    post {
        always {
            echo 'Slack Notifications.'
            slackSend channel: '#cicd1',
                color: COLOR_MAP[currentBuild.currentResult],
                message: "*${currentBuild.CurrentResult}:* Job ${env.JOB_NAME} build ${env.BUILD_NUMBER} \n More info at: ${env.BUILD_URL}"
        }

    }
>>>>>>> 2360a9eea58c5c9265679ade9561c647818789c6
}
