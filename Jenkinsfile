node{
  stage ('SCM Checkout') {
    git 'https://github.com/jenkins-docs/simple-java-maven-app'
  }
  stage ('Compile-Package'){
  sh 'mvn package'
  }
}
