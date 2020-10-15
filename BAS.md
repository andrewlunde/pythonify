mkdir -p /home/user/projects
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
echo "export PATH=$PATH:/home/user/usr/bin:/home/user/usr/local/bin" >> ~/.bashrc
echo "" >> ~/.bashrc
echo "Restart Bash."
curl -LJO https://bootstrap.pypa.io/get-pip.py
python get-pip.py --prefix=/home/user
python -m pip install --upgrade pip
python -m pip install --upgrade setuptools
python -m pip install --upgrade wheel
pip --version
pip install cfenv