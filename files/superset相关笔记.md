https://github.com/shbokesoft/superset/blob/master/CONTRIBUTING.md

```
# Create a virtual environment and activate it (recommended)
python3 -m venv venv # setup a python3 virtualenv
source venv/bin/activate

# Install external dependencies
pip install -r requirements/local.txt

# Install Superset in editable (development) mode
pip install -e .

# Create an admin user in your metadata database
superset fab create-admin

# Initialize the database
superset db upgrade

superset init

superset load-examples

FLASK_ENV=development superset run -p 8088 --with-threads --reload --debugger
```

笔记： npm/6.11.3   node/12.12.0
报错sasl.h找不到
https://www.lfd.uci.edu/~gohlke/pythonlibs/ 
下载对应的sasl.whl文件  
在对应目录下安装 pip install xxm-win_amd64.whl


https://www.cnblogs.com/twodog/p/12136034.html

数据库链接配置时 clickhouse://default:abcd1234@1.1.1.33:8123/erp_test

如果数据库连接测试不通过  可能是 需要 "pip install clickhouse-sqlalchemy  (setup.py里面有)

# clean-webpack-plugin各版本踩坑记

https://blog.csdn.net/achuan87/article/details/104723051/