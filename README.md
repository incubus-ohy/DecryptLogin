# DecryptLogin
```
APIs for loginning some websites using <requests>.
You can star this repository to keep track of the project if it's helpful for you, thank you for your support.
```

# Introduction in Chinese
https://mp.weixin.qq.com/s/lctw2dGjOesXrfvkNhzYfQ
#### Some Examples
- weiboMonitor: https://mp.weixin.qq.com/s/uOT1cGqXkOq-Hdc8TVnglg

# Support List
|  Websites        | support PC API?                     |  support mobile API?              |
|  :----:          | :----:                              |  :----:                           |
|  weibo           | No                                  |  [Yes](./src/platforms/weibo.py)  |
|  douban          | [Yes](./src/platforms/douban.py)    |  No                               |
|  GitHub          | [Yes](./src/platforms/github.py)    |  No                               |
|  Music163        | [Yes](./src/platforms/music163.py)  |  No                               |
|  12306           | [Yes](./src/platforms/zt12306.py)   |  No                               |
|  QQZone          | No                                  |  [Yes](./src/platforms/QQZone.py) |
|  QQQun           | No                                  |  [Yes](./src/platforms/QQQun.py)  |

# Install
### Use setup.py
#### Step1
```sh
git clone https://github.com/CharlesPikachu/DecryptLogin.git
```
#### Step2
```sh
cd DecryptLogin -> run "python setup.py install"
```
### Use pip
```sh
pip install git+https://github.com/CharlesPikachu/DecryptLogin.git@master
```

# Usage
#### Example
```python
from DecryptLogin import login
lg = login.Login()
session = lg.douban(username[telephone], password, 'pc')
session = lg.github(username[email], password, 'pc')
session = lg.weibo(username[telephone], password, 'mobile')
session = lg.music163(username[telephone/email], password, 'pc')
session = lg.zt12306(username[telephone], password, 'pc')
session = lg.QQZone('mobile')
session = lg.QQQun('mobile')
```
#### Arguments
```
username: your username.
password: your password.
version: pc/mobile.
```

# More
#### WeChat Official Accounts
*Charles_pikachu*  
![img](./pictures/pikachu.jpg)