由于rabbitmq是很久以前学的了，很多知识都忘记了，回来重新复习一下。先从搭建开始，逐步复习。

* docker安装rocket mq

```bash
docker pull rabbitmq

docker run -d \
--hostname my-rabbit --name rabbit \
-e RABBITMQ_DEFAULT_USER=admin -e RABBITMQ_DEFAULT_PASS=admin \
-p 15672:15672 -p 5672:5672 \
-v /data:/home/rabbitmq \
rabbitmq
```

