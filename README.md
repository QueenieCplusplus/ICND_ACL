# ICND_ACL
IP Access Control

# CLI

基本的存取控制指令：

* access-list 

* ip access-group


範例：

     router(config)# access-list + < access-list-number> + permit 
     // 存取清單中包含了辨識封包的一般性敘述。
     
     router(config)# access-list + < access-list-number> + deny
     
     router(config)# < protocol > + access-group + < access-list-number>  + in
     // 將一份存取清單指定給予一介面。

     router(config)# < protocol > + access-group + < access-list-number>  +  out
     
