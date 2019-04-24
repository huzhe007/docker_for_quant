## Anaconda

#### 安装运行

```shell
docker pull continuumio/anaconda3

docker run -i -t -p 8888:8888 continuumio/anaconda3 /bin/bash -c "/opt/conda/bin/conda install jupyter -y --quiet && mkdir /opt/notebooks && /opt/conda/bin/jupyter notebook --notebook-dir=/opt/notebooks --ip='*' --port=8888 --no-browser"
```



#### 参考资料

+ [continuumio/anaconda3](https://hub.docker.com/r/continuumio/anaconda3)
+ [anaconda3](<https://github.com/ContinuumIO/docker-images/tree/master/anaconda3>)

