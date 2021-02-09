node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'idxdocker') {

        def customImage = docker.build("idx-manage:${env.BUILD_ID}")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
