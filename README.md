# wso2_mi_sample
Basic transformation and enrichment sample.

## Start mi on docker
```docker run -p 127.0.0.1:8253:8053 -p 127.0.0.1:8290:8090 *irosales/training*```


## enable CLI on docker conainer start

```docker run -p 127.0.0.1:8253:8253 -p 127.0.0.1:8290:8290 -p 127.0.0.1:9164:9164 -e JAVA_OPTS="-DenableManagementApi=true"  irosales/training```


## login to micro integration


```mi remote login admin admin``` where admin / admin is the default user and password.

## Show API details

```
mi api show
  NAME       URL
  HelloAPI   http://localhost:8290/sayHello

mi api show HelloAPI
Name - HelloAPI
Version - N/A
Url - http://localhost:8290/sayHello
Stats - disabled
Tracing - disabled
Resources :
  URL       METHOD
  /{name}   GET
```



