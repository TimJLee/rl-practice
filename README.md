# rl-practice
캡스톤 대비 강화학습 스터디

## Setting
pull docker image & make container on it
```
> docker pull jaimeps/rl-gym
> docker images
> docker run -it -p 8888:8888 -e GRANT_SUDO=yes --user root --name openAI jaimeps/rl-gym
> docker stop openAI
> docker ps
> docker ps -a
> docker start openAI
> docker ps
> docker stop
```
if error occured on container
```
> docker rm openAI
> docker ps -a
> docker run -it -p 8888:8888 -e GRANT_SUDO=yes --user root --name openAI jaimeps/rl-gym
```
then go to [http://localhost:8888](http://localhost:8888)
> make sure you have to put token in password **only first try**
> WARN : don't change docker power setting after pulling images or making containers.. they are gonna all gone if setting changed. make sure you change docker power setting(allow CPU to 8 etc..) **only at right after Docker install**  

Install additional dependencies and restart container  
-terminal
```
# pip3 install box2d box2d-kengz
# pip3 install jupyter-tensorboard
```
-cmd
```
> docker stop openAI
> docker start openAI
```
