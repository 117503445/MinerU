cd docker/china
docker build -t registry.cn-hangzhou.aliyuncs.com/117503445/mineru .
docker run --rm -it --gpus=all registry.cn-hangzhou.aliyuncs.com/117503445/mineru /bin/bash -c "echo 'source /opt/mineru_venv/bin/activate' >> ~/.bashrc && exec bash"
docker push registry.cn-hangzhou.aliyuncs.com/117503445/mineru