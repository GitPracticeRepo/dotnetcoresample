node {
    stage('VCS') {
        git branch: 'master', url: https://github.com/GitPracticeRepo/dotnetcoresample.git
    }
    stage('build') {
        println "building code"
        sh 'dotnet build'
    }
}