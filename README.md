# Cluster-Using-NodeJS
## Steps:

1.**clone the repository**

2.**Start the server**
```
node index.js
```
```
 Note:In this example the cluster module is used to run the server code in more than one CPU.
 .
 .
 .
 if(cluster.isMaster){

        //Fork the process                
        for(let cpu of os.cpus()){
                cluster.fork()
        }
}else{
        serverFcn()
}
```
