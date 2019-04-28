## Anaconda

#### 安装运行

##### docker

```shell
docker pull continuumio/anaconda3

docker run -i -t continuumio/anaconda3 /bin/bash
docker run -i -t -p 8888:8888 continuumio/anaconda3 /bin/bash -c "/opt/conda/bin/conda install jupyter -y --quiet && mkdir /opt/notebooks && /opt/conda/bin/jupyter notebook --notebook-dir=/opt/notebooks --ip='*' --port=8888 --no-browser"
```

##### OSX

```shell
# 安装
双击 Anaconda3-2019.03-MacOSX-x86_64.pkg
# 卸载
cd ~/anaconda3/bin
./conda install anaconda-clean
./anaconda-clean
rm -r ~/.anaconda_backup
rm -rf ~/anaconda3
rm -rf ~/.condarc ~/.conda ~/.continuum
```

#### 参考资料

+ [continuumio/anaconda3](https://hub.docker.com/r/continuumio/anaconda3)
+ [anaconda3](https://github.com/ContinuumIO/docker-images/tree/master/anaconda3)
+ [《Mac系统下基于Anaconda3安装Python集成开发环境》](https://blog.csdn.net/zzl819954692/article/details/80223861)
+ [《Installing on macOS》](https://docs.anaconda.com/anaconda/install/mac-os/#)