node {
   def mvnHome
  stage('Prepare') {
      git url: 'https://github.com/Royal-Reddy-Yaparla/my_java_web_application_02.git', branch: 'main'
      mvnHome = tool 'maven'
   }
//     stage ('Code Analysis') {
//       sh "'${mvnHome}/bin/mvn' sonar:sonar"
//   }
  stage ('Clean') {
      sh "'${mvnHome}/bin/mvn'  clean"
  }
  stage ('Validate') {
      sh "'${mvnHome}/bin/mvn'  validate"
  }
  stage ('Compile') {
      sh "'${mvnHome}/bin/mvn'  compile"
  }
  stage ('Test') {
      sh "'${mvnHome}/bin/mvn'  test"
  }
  stage ('Package') {
      sh "'${mvnHome}/bin/mvn'  package"
  }
  stage ('Verify') {
      sh "'${mvnHome}/bin/mvn'  verify"
  }
  stage ('Install') {
      sh "'${mvnHome}/bin/mvn'  install"
  }
//   stage ('Deliver & Deployment') {
//       sh 'curl -u admin:redhat@123 -T target/**.war "http://18.212.151.66:8080/manager/text/deploy?path=/Royal&update=true"'
//   }
//   stage ('SmokeTest') {
//       sh 'curl --retry-delay 10 --retry 2 "http://18.212.151.66:8080/Royal"'
//   }

}