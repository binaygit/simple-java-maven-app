node{
  env.JAVA_HOME = tool name: 'java', type: 'jdk'
  def mvnHome = tool name: 'maven3', type: 'maven'
  def mvnCMD = "${mvnHome}/bin/mvn"
  stage('SCM Checkout'){
  git 'https://github.com/binaygit/simple-java-maven-app/'
   }
  stage('Compile'){
    echo "Compiling the Source code"
    sh "${mvnCMD} compile"
  }
stage('Package'){
   /* def mvnCMD = "${mvnHome}/bin/mvn" */
  echo "Package the source code"
  sh "${mvnCMD} package"
  }
}
