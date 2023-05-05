# podman-fedora-nvidia


How to use

```bash
# You must provide the following lines:
# --security-opt=label=disable
# --hooks-dir=/usr/share/containers/oci/hooks.d/

podman run --rm -it \
    --security-opt=label=disable \
    --hooks-dir=/usr/share/containers/oci/hooks.d/ \
    docker.io/nvidia/cuda:11.6.2-base-ubuntu20.04

# (inside the container)
nvidia-smi
```