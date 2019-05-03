node {
    stage ('Hello'){
        echo 'Hello World'
    }
    stage ('Checkout'){
        git 'https://github.com/eugenerainey/jenkinstesting.git'
    }
    stage ('Clean'){
        sh "./gradlew clean"
    }
    stage ('Build'){
        sh "./gradlew assembleDebug"
    }
    stage ('Test'){
        sh "./gradlew testDebugUnitTest"
    }


}