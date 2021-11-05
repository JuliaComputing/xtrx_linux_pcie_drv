# xtrx_linux_pcie_drv
XTRX PCI driver for linux 

```
mkdir -p build
cd build
cmake -DCMAKE_INSTALL_PREFIX:PATH=/usr ..
sudo make install
# Note the version should be set approriately in CMakeLists.txt and dkms.conf
sudo dkms add -m xtrx -v "0.2.0-1"
sudo dkms build -m xtrx -v "0.2.0-1"
sudo dkms install --force -m xtrx -v "0.2.0-1"
```