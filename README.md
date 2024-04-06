<p align="center">
  <img src="https://github.com/akromovx/GLVM/blob/main/logo/figma_frame_glvm.png?raw=true" alt="Sublime's custom image"/>
</p>

# Game Loop Versatile Modules (GLVM)

<p style="text-align: center;">Game Loop Versatile Modules - GLVM</p>

Simple Game Engine for Windows and Linux Operating Systems with support OpenGL and Vulkan, based on Entity component system

# Assets Support

Models

 - GLTf
 - wavefront (.obj)

Sounds

- wav

# Build

## Windows

For build GLVM you need installed [MSYS2](https://www.msys2.org/)

#### 1. Install pacboy
```pacman -S pactoys```
#### 2. Install dependencies
``pacboy -S gcc:p``

``pacboy -S vulkan:p``
#### 3. Build
``make -f MakefileWin``



## Linux

### 1. Install dependencies
#### Gentoo
        emerge --ask x11-libs/libX11 \
                     x11-libs/libXi \
                     x11-apps/xrandr \
                     media-libs/vulkan-loader \
                     dev-util/vulkan-tools \
                     media-libs/mesa \
                     media-libs/alsa-lib \
                     media-sound/pulseaudio

#### Debian
        apt install libx11-dev \
                    libxi-dev \
                    libxrandr-dev
                    libgl1-mesa-dev \
                    libasound2-dev \
                    libpulse-dev \
                    libudev-dev

#### Arch
        pacman -S libxi \
                  libxrandr \
                  mesa \
                  libglvnd \
                  alsa-lib \
                  pulseaudio

#### Fedora
        dnf install libX11-devel \
                    libXrandr-devel \
                    libXi-devel \
                    mesa-libGL-devel \
                    alsa-lib-devel \
                    pulseaudio-libs-devel \
                    libudev-devel \
                    libstdc++-static

### 2. Build
``make -f MakefileLin``


# License
Copyright © 2024 Maksim Manokhin a.k.a. Yuriorkis_Scream. Contacts: <fellfrostqtw@gmail.com>
