helm upgrade sn . -n sn   --set global.resources.requests.memory="64Mi"   --set global.resources.requests.cpu="250m"   --set global.resources.limits.memory="128Mi"   --set global.resources.limits.cpu="1" --set global.replicas=4

python3 scripts/init.py --compose（初始化脚本，一定要加--compose

让jaeger正常工作  (Changing the imageVersion to 1.62.0)

nginx

command:

    - /bin/sh
    
    - -c
    
  args:
  
    - |

      git -c http.proxy=http://10.112.80.105:7890 \
      
          -c https.proxy=http://10.112.80.105:7890 \
          
          clone https://github.com/yzz9048/DeathStarBench_File.git /DeathStarBench


      cp -r /DeathStarBench/gen-lua/* /gen-lua/
      
      cp -r /DeathStarBench/openresty-thrift/lua-thrift/* /lua-thrift/
      
      cp -r /DeathStarBench/nginx-web-server/lua-scripts/* /lua-scripts/
      
      cp -r /DeathStarBench/nginx-web-server/pages/* /pages/
      
      cp /DeathStarBench/keys/* /keys/

media-frontend

# the same operation for git as nginx

 cp -r /DeathStarBench/lua-scripts/* /lua-scripts/
