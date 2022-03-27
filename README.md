# backport-iwlwifi
intel wifi driver backport
intel WiFi firmware binaries  


# First, install some necessary package

sudo apt install flex bison

# Compile and install it:

git clone https://github.com/intel/backport-iwlwifi.git

cd iwlwifi-stack-dev

sudo make defconfig-iwlwifi-public

sudo make 

sudo make install

# Finally, copy the fw-binaries
sudo cp ../fw-binaries/iwlwifi-* /lib/firmware/
