node{
  stage('SCM Checkout'){
  git 'https://github.com/binaygit/simple-java-maven-app/'
}
stage('Compile Package'){
  def mvnHome = tool name: 'maven-3', type: 'maven'
  def mvnCMD = "${mvnHome}/bin/mvn"
  sh "${mvnCMD} package"
  }
}
