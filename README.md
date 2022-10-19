# flask_tutorial
https://flask.palletsprojects.com/en/2.2.x/quickstart/ 代码

## 运行

将代码克隆到本地以并进入`flask_tutorial`目录后，运行下面命令安装所需依赖包
`pip install -r requirements.txt`

等安装完所需依赖后，运行一下命令，以开发模式启动
```
flask --app flaskr --debug run
```
出现一下输出，则表明成功运行
```
* Debug mode: on
WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
 * Running on http://127.0.0.1:5000
Press CTRL+C to quit
 * Restarting with watchdog (windowsapi)
 * Debugger is active!
 * Debugger PIN: 231-118-413
```

打开浏览器后，会出现下面情况

![image](https://user-images.githubusercontent.com/81068011/196604182-76279654-f9c1-4165-9d47-793c07b82d2e.png)

这是因为还未初始化数据库导致的。所有需要先初始化数据库，命令如下：
```
$ flask --app flaskr init-db
Initialized the database.
```
然后再次运行启动命令即可。

![image](https://user-images.githubusercontent.com/81068011/196606937-c31566d7-5906-4cd1-ac59-1b2dc70d1c74.png)


其他更详细的内容，请查看 [Tutorial — Flask Documentation (2.2.x)](https://flask.palletsprojects.com/en/2.2.x/tutorial/)
