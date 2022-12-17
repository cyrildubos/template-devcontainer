# Template - Dev Container

A Dev Container template for Arch Linux, X11, NVIDIA, and more...

## NVIDIA Container Toolkit

On the host machine, install NVIDIA Container Toolkit package:

```console
paru -S nvidia-container-toolkit
```

In the Dev Container, install `nvidia-utils` package:

```console
pacman -S --overwrite \* nvidia-utils
```

### With a laptop as the host machine

In the Dev Container, install `nvidia-prime` package:

```console
pacman -S nvidia-prime
```

Then, run programs on NVIDIA GPU with the `prime-run` script:
```console
prime-run [program]
```
