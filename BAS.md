```
mkdir -p /home/user/projects
git config --global user.email "andrew.lunde@sap.com"
git config --global user.name "Andrew Lunde"
cd ~
curl -LJO http://thedrop.sap-partner-eng.com/files/python3.tgz
tar xzvf python3.tgz
cd usr/bin
ln -s python3.7 python
cd projects
git clone https://github.com/andrewlunde/pythonify.git
cd ~
echo "" >> ~/.bashrc
echo "export LD_LIBRARY_PATH=/lib/x86_64-linux-gnu:/home/user/lib" >> ~/.bashrc
echo "export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/home/user/usr/lib" >> ~/.bashrc
echo "export PATH=$PATH:/home/user/usr/bin:/home/user/usr/local/bin:/home/user/bin" >> ~/.bashrc
echo "" >> ~/.bashrc
echo "Restart Bash."
cd ~
curl -LJO https://bootstrap.pypa.io/get-pip.py
python get-pip.py --prefix=/home/user
cd bin


AHHHHHH I HAD IT WORKING!!!!!!
/home/user/.local ??

https://packaging.python.org/tutorials/installing-packages/


user: python $ python -m pip install --upgrade pip setuptools wheel
Requirement already up-to-date: pip in /home/user/.local/lib/python3.7/site-packages (20.2.3)
Collecting setuptools
  Using cached setuptools-50.3.1-py3-none-any.whl (785 kB)
Collecting wheel
  Using cached wheel-0.35.1-py2.py3-none-any.whl (33 kB)
Installing collected packages: setuptools, wheel
Successfully installed setuptools-50.3.1 wheel-0.35.1

user: python $ pip install sap_xssec 
Collecting sap_xssec
  Downloading sap_xssec-2.1.0-py2.py3-none-any.whl (15 kB)
Requirement already satisfied: six>=1.11.0 in /home/user/usr/local/lib/python3.7/dist-packages (from sap_xssec) (1.15.0)
Collecting deprecation>=2.1.0
  Downloading deprecation-2.1.0-py2.py3-none-any.whl (11 kB)
Collecting requests>=2.21.0
  Downloading requests-2.24.0-py2.py3-none-any.whl (61 kB)
     |████████████████████████████████| 61 kB 981 kB/s 
Collecting pyjwt>=1.7.0
  Downloading PyJWT-1.7.1-py2.py3-none-any.whl (18 kB)

File "/home/user/usr/local/lib/python3.7/dist-packages/flask/app.py"

python -m pip install --upgrade pip
python -m pip install --upgrade setuptools
python -m pip install --upgrade wheel
pip --version
pip install cfenv
```
