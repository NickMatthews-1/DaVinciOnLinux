# DaVinciOnLinux
This is a install instructions repo for how to install Resolve on Debian.

### Step 1
Update your system

### Step 2
Download and extract the DaVinci Resolve ZIP from the website

### Step 3
Make the DaVinci Resolve run file executable with
```
chmod +x ./DaVinci_Resolve_18.1.1_Linux.run
```

### Step 4
Run the DaVinci Resolve executable with
```
./DaVinci_Resolve_18.1.1_Linux.run
```

### Step 5
WHen the dialog box pops up telling you what you are missing copy the missing items and install them.

### Step 6
Download the AMD GPU Drivers from AMD with the following
```
wget https://drivers.amd.com/drivers/linux/amdgpu-pro-20.40-1147286-ubuntu-20.04.tar.xz --referer https://www.amd.com/en/support/kb/release-notes/rn-amdgpu-unified-linux-20-40
```

### Step 7
Extract the AMD GPU Drivers tar using the following
```
tar -xJpf amdgpu-pro-20.40-1147286-ubuntu-20.04.tar.xz 
```

### Step 8

Run the GPU install command in the following format

```
./amdgpu-install --opencl=legacy --headless --no-dkms
```

### Step 9
Once the AMD GPU Drivers are installed go back to DaVinci Resolve and run the installer again

### Step 10
Upon the install of DaVinci Resolve run it and you have a working install

### Disclaimer
There is not gurantee this will work on Debian systems as DaVinci was aimed at CentOS and it has caused alot of issues because of this fact so there is no 100% chance it will work. If it does then everything will be fantastic. If not then there isnt much that can be done as Black Magic Design will not be offering support.
