branch_name=githubashim

node {
    checkout scm

    docker.withRegistry('https://github.com/ashimgrg/docker-react.git', ${env.branch_name}) {

        def customImage = docker.build("ashimgrg/docker-react")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
