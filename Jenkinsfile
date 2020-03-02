node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'nbawaDockerHub') {

        def customImage = docker.build("neelam/nodeapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}