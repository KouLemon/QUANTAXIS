# QUANTAXIS 的安装 MAC篇

<!-- vscode-markdown-toc -->
* 1. [python](#python)
* 2. [QUANTAXIS](#QUANTAXIS)
* 3. [MONGODB](#MONGODB)
* 4. [NODEJS](#NODEJS)
* 5. [QUANTAXIS_WEBKIT](#QUANTAXIS_WEBKIT)

<!-- vscode-markdown-toc-config
	numbering=true
	autoSave=true
	/vscode-markdown-toc-config -->
<!-- /vscode-markdown-toc -->
##  1. <a name='python'></a>python
```
brew install python3
```

##  2. <a name='QUANTAXIS'></a>QUANTAXIS

```
git clone https://github.com/yutiansut/quantaxis --depth 1
cd quantaxis .
sudo python3.6 -m pip install -r requirements.txt -i https://pypi.doubanio.com/simple
sudo python3.6 -m pip install tushare
sudo python3.6 -m pip install pytdx

python3.6 -m pip install -e .
```


##  3. <a name='MONGODB'></a>MONGODB

安装mongodb:
```
brew update
brew install mongodb
```


创建数据库文件:
```
sudo mkdir -p /data/db
```

然后需要输入你的密码

启动mongodb
```
sudo mongod
```
继续输入你的密码


##  4. <a name='NODEJS'></a>NODEJS

```
brew install node

sudo npm install cnpm -g
sudo npm install forever -g
```

##  5. <a name='QUANTAXIS_WEBKIT'></a>QUANTAXIS_WEBKIT

```
cd QUANTAXIS_WEBKIT\web 
cnpm install

cd QUANTAXIS_WEBKIT\backend
cnpm install
```