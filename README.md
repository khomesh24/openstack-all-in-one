# openstack-architecture 


                                                    |
                                                    | eth0 - Public IP (192.168.124.95) // Internet facing // Full internet access
                                                    |    
                                        +-----------+-----------+  
                                        |                       |
                                        |                       |
                                        |      Host_System      |   
                                        |                       |
                                        |     Openstack Env     |
                                        +-----------+-----------+  
                                       		    | 
                                                 Nating 
                                                    |       
                    +--------------------------------+--------------------------+
                    |                                                           |                            
                    |                                                           |
                    |  eth0-10.0.0.20 (Private-Net-IP) 				| eth0- 10.0.0.30 (Private-Net-IP)
                    |	    192.168.124.0 (Floating-IP)		          	|	192.168.124.0 (Floating-IP)		
         +-----------+-----------+                                  +-----------+-----------+                                  
         |                       |                                  |                       |
         |                       |                                  |                       |
         |        VM-1           |                                  |          VM-2         |
         |                       |                                  |                       |
         |                       |                                  |                       |
         +-----------+-----------+                                  +-----------+-----------+ 


