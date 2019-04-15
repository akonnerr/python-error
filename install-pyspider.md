### pip install pyspider时出现报错
```python
"python setup.py egg_info" failed with error code 1 in /private/var/folders/b7/r2gh1q256wj_tg77fp8y5wgr0000gn/
T/pip-install-aprnjrct/Pycurl/
```
### 解决方案
```python
export LDFLAGS=-L/usr/local/opt/openssl/lib
export CPPFLAGS=-I/usr/local/opt/openssl/include
export PYCURL_SSL_LIBRARY=openssl
#将openSSL配置到环境
```
