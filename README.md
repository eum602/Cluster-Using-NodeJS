# Cluster-Using-NodeJS
## Steps:

1.**clone the repository**

2.**Start the server**
```
node index.js
```
```
 Note:
 if(cluster.isMaster){

        //Fork the process                
        for(let cpu of os.cpus()){
                cluster.fork()
        }
}else{
        serverFcn()
}
```
