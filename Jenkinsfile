node {
   def mvnHome
  stage('Prepare') {
      git url: 'https://github.com/Msupriya1506/b810am.git', branch: 'main'
      mvnHome = tool 'maven'
   }
  
  stage ('Clean') {
      sh "'${mvnHome}/bin/mvn' clean"
  }
  stage ('Validate') {
      sh "'${mvnHome}/bin/mvn' validate"
  }
  stage ('Compile') {
      sh "'${mvnHome}/bin/mvn' compile"
  }
  stage ('Test') {
      sh "'${mvnHome}/bin/mvn' test"
  }
  stage ('Install') {
      sh "'${mvnHome}/bin/mvn' install"
  }
  stage ('Verify') {
      sh "'${mvnHome}/bin/mvn' verify"
  }
  stage ('deploy') {
      sh "'${mvnHome}/bin/mvn' deploy"
  }
}