node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'nbawaDockerHub') {

        def customImage = docker.build("neelubawa/mynodeapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
