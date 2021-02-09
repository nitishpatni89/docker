node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'idxdocker') {

        def customImage = docker.build("nitish1989/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
