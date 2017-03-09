stage 'Ballin'
node {
  checkout scm
  sh 'echo $BRANCH_NAME'
}
if (env.BRANCH_NAME == 'master') {
  stage 'Only on master'
  println 'This happens only on master'
} else {
  stage 'Feature branch build'
  println "Current branch ${env.BRANCH_NAME}"
  stage 'Feature branch deploy'
  println "Deploying ${env.BRANCH_NAME}"
  stage 'Feature branch promote'
  println "Deploying ${env.BRANCH_NAME}"
}
