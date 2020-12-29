K8s with single container.

To have k8s use new image after making code changes,
- tag the new image with a version and push to dockerhub
- one option: change the deployment config file to specify the new new image, and then run kubectil apply.
- 2nd option: imperatively updating without change config file by using kubectl set command. See notes folder.

However, the best option is to use $GIT_SHA (git commit id) to tag the image. See multi-k8s course.
