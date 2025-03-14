# RUOYI-CLOUD in docker

## Build RuoYi Micro-service version
+ Under “RunYi-Cloud" folder, run mvn command to build all micro-service jar packages  
    ```bash
    mvn clean package
    ```  

## Build RuoYi frontend
+ Under "RuoYi-Cloud-Vue3", run yarn command to pack latest UI package  
    ```bash
    yarn build:prod
    ```  

+ Copy dist folder from folder "RuoYi-Cloud-Vue3" to folder "RuoYi-Cloud/ruoyi-ui"  

## Start RUOYI Micro-service version in single host
Under folder "RuoYi-Cloud/docker", run docker-compose command to start Micro-service version in single host:  

    ```bash
    docker-compose up -d
    ```  

## Open RuoYi

### RuoYi Frontend
http://ruoyi.atool.localhost/  

> Default account: admin/admin123  

### Sentinel
+ Build image  
    ```bash
    docker build -t sentienl:latest -f dockerfile .
    ```  

+ Run image
    ```bash
    docker run -d -it -p 8888:8080 --name sentinel sentienl:latest
    ```  

    > Default account: sentinel/sentinel  

    > https://sentinelguard.io/zh-cn/docs/introduction.html  

## Nacos
http://nacos.ruoyi.atool.localhost/

> No password  

## Monitor
http://monitor.ruoyi.atool.localhost/

> Default account: ruoyi/123456  

> https://doc.ruoyi.vip/ruoyi-cloud/cloud/monitor.html#%E5%9F%BA%E6%9C%AC%E4%BB%8B%E7%BB%8D  


