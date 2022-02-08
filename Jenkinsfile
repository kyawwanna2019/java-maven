node {
    def app

    stage('Clone repository') {
       checkout scm
    } 
    stage('Generate Jar Package') {
            //dir("/var/lib/jenkins/workspace/New_demo/my-app/") {
                def pom = readMavenPom file:'pom.xml'
                sh 'mvn -B -DskipTests clean package'
            //} 
    }   
}