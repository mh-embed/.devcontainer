# Devcontainer Docs

# Add devcontainer

To Add this devcontainer config to your dev environment, either clone this repo, or go to your git repository, then run
```
git submodule add https://github.com/mh-embed/.devcontainer/ .devcontainer/
```
This adds the drone-devcontainer-buster repo to your git repo as a submodule in the path .devcontainer, which is recognized by VSCode.

# Get devcontainer in VSCode
1. Make sure you have docker
```
docker --help
```

2. Pull the docker image of your platform: 
- If you have a x86_64(AMD64) machine (most Windows/Linux laptops and desktops), run
```
docker pull danielhouevr315/rone-devcontainer-buster:amd64
```
- If you have an arm v8 64 bit device (a Mac with Apple Silicon, etc)
```
docker pull danielhouevr315/rone-devcontainer-buster:arm64
```
*Warning: * arm64 image is designed for 64 bit ARM dev environments, it may not run on a Raspberry Pi with 32 bit OS. 

3. Add devcontainer as described in the previous section. When you see the .devcontainer folder in your project, VSCode may prompt you to repoen the project in devcontainer. 
- Make sure you installed the devcontainer extension to VSCode
- If not prompted, click the bottom left green button and select "Repoen in Devcontainer". 
- When done testing, click the bottom left green button and select "Repoen folder locally" to return to your host machine in terminal. 

# Develop in ROS devcontainer

