node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'idxdockergit') {

        def customImage = docker.build("nitish1989/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
