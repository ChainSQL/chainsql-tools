# chainsql-tools 
ChainSQL Tools 用来辅助用户使用ChainSQL产品，如生成配置文件等

## 生成配置文件
```
用法: java -classpath chainsql-tools.jar com.peersafe.genChainsqlCfg -m args -n args
 -m,--multi <arg>    -m 可选项，表示要生成多个节点（不同ip）的配置文件，多个ip间用分号';'隔开
 -n,--number <arg>   -n 必选项，指定要生成的配置文件数量
```

示例1，单点生成4个配置文件，端口不同
```
java -classpath chainsql-tools.jar com.peersafe.genChainsqlCfg -n 4
```

示例2 ，4个IP地址，每个IP一个配置文件
```
java -classpath chainsql-tools.jar com.peersafe.genChainsqlCfg -m "192.168.29.100;192.168.29.101;192.168.29.102;192.168.29.103" -n 4
```
