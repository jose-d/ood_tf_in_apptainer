## build base image

This apptainer image is based on https://hub.docker.com/r/tensorflow/tensorflow/ docker image.

(sudo needed?)

```
sudo apptainer build --nv ./tf_from_docker_base.sif ./tf_from_docker_base.def
```

## build top level image

without sudo

```
apptainer build --nv ./tf.sif ./tf_from_docker_install_exts.def
```
