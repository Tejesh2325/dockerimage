node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'TejaDocker') {

        def customImage = docker.build("tejeshinfo5/dockerimageTeja$BUILD_NUMBER")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
