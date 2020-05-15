node {
    stage('VCS') {
        git branch: 'master', url: 'https://github.com/GitPracticeRepo/dotnetcoresample.git'
    }
    stage('build') {
        println "building code"
        sh 'dotnet build'
    }
    stage('archive'){
        archiveArtifacts 'bin/Debug/netcoreapp3.1/dotnetcoresample'
    }
}