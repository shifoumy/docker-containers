Gitlab Runner execution
-----------------------

Show this documentation : https://docs.gitlab.com/runner/install/docker.html

Tips :
As your CLI container or gitlab-ci-runner container need to mount the host machine's Docker socket in the container. This will allow your container to use the host machine's Docker daemon to run containers and build images.

Source : https://stackoverflow.com/a/52696951

We need to add `"/var/run/docker.sock:/var/run/docker.sock"` in volume list into runner cofiguration.


See https://gitlab.com/gitlab-org/gitlab-runner/-/issues/4566#note_221034749 discution for more informations
