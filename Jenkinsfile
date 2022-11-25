node{
  stage('SCM checkout'){
    git 'https://github.com/Swanandd55/git'
  }
  stage('Compile-Package'){
    def mvnHome = tool name: 'maven-3', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }
  stage('Email Notification'){
    mail bcc: '', body: 'hello jenkins', cc: '', from: '', replyTo: '', subject: 'jenkins job', to: 'swanand2397@gmail.com'
  }
}
