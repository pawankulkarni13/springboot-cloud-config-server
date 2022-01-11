# springboot-cloud-config-server

Sample application to demonstrate cloud config server, which in this case picks from a local directory file.
It can be customized to pick from Git location as needed.

Urls--
http://localhost:8888/application-dev.json
http://localhost:8888/application/dev


Note: if application complain about git in app-config, execute below in local
Goto App-config in terminal console.
git init
git add --all
git commit -m "initial configs"

Come back and run the application. It should work fine now.!

If git complain while commit about app-config
git rm --cached app-config
git submodule add ./ app-config
