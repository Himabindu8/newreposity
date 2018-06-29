node{
stages{
   stage('Clone')
   {
   chekout scm
   }
   stage('Build')
   {
   bat 'mvn -s $MAVEN_SETTINGS -B clean deploy cobertura:cobertura javadoc:javadoc'
   }
   }
   }
