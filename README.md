# k8s_study

## key commands
```
export PATH=$PATH:/usr/local/go/bin
su - developer

kubectl delete all --all --all-namespaces

docker run --name pd -p 2379:2379 -p 2380:2380 pingcap/pd
docker run --name tikv -p 20160:20160 pingcap/tikv --pd="localhost:2379"
docker run --name tidb -p 4000:4000 -p 10080:10080 pingcap/tidb --path="localhost:2379"

mysql -h 127.0.0.1 -P 4000 -u root -D test
```


## good tutorial
总体流程
```
https://book-v1.book.kubebuilder.io/basics/project_creation_and_structure.html
```

deploy tidb with kubenetes
```
https://docs.pingcap.com/tidb-in-kubernetes/dev/get-started
```

一个简单的hello world级别的project
```
https://dev.to/ishankhare07/writing-a-simple-kubernetes-controller-in-go-with-kubebuilder-ib8
```

## b站教学
相关资料
```
https://docs.google.com/document/d/1qRZGDnUTmORMRbtrQRCMSUcItur5-5jjpKZy_bTZIQo/edit
```