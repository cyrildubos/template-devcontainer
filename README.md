# Template - Dev Container

## NVIDIA Container Toolkit

On the host machine, install NVIDIA Container Toolkit package :

```console
pacman -S nvidia-container-toolkit
```

### With a laptop as the host machine

In the Dev Container, install `nvidia-utils` and `nvidia-prime` packages :

```console
pacman -S --overwrite \* nvidia-utils
pacman -S nvidia-prime
```

Then, run programs on the NVIDIA GPU with the `prime-run` script :
```console
prime-run [program]
```
