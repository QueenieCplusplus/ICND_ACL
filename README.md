# ICND ACL
IP Access Control List

# CLI

基本的存取控制指令：

* access-list 

* ip access-group


範例：

     router(config)# access-list + < access-list-number> + permit 
     // test, 存取清單中包含了辨識封包的一般性敘述。
     
     router(config)# access-list + < access-list-number> + deny
     // test
     
     router(config)# access-list + < access-list-number> + permit + src add/wildcard mask
     // 預設為 mask 0.0.0.0，全部比對。
     
     router(config)#int + <介面與介面編號>
     
     router(config-if)#ip-access-group + < access-list-number>  + in
     
     router(config-if)#ip-access-group + < access-list-number>  + out
     
     router(config)# < protocol > + access-group + < access-list-number>  + in
     // 將一份存取清單指定給予一介面。

     router(config)# < protocol > + access-group + < access-list-number>  +  out
     
