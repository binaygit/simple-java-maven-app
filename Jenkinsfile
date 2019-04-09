node{
  stage('SCM Checkout'){
  git 'https://github.com/binaygit/simple-java-maven-app/'
}
stage('Compile Package'){
  def mvnHome = tool name: 'maven3', type: 'maven'
   /* def mvnCMD = "${mvnHome}/bin/mvn" */
  sh "${mvnHome}/bin/mvn package"
  }
}
