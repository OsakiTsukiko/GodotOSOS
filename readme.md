### WIP
  
# GodotOSOS
### What is it?
Its basically a small operating system build around the godot project GodotOS by popcar2 based on Arch Linux. (made with archiso)

### How to build
Arch Wiki: https://wiki.archlinux.org/title/archiso  
  
```bash
# you might need to be on arch (idk) and you need archiso installed
git clone https://github.com/OsakiTsukiko/GodotOSOS
cd GodotOSOS
mkdir workdir
sudo mkarchiso -v -w ./workdir ./sauce/

# Warning: If mkarchiso is interrupted, run findmnt(8) to make sure 
# there are no mount binds before deleting it - otherwise, you may 
# lose data (e.g. an external device mounted at /run/media/user/label 
# gets bound within work/x86_64/airootfs/run/media/user/label during 
# the build process).
rm -rf workdir
```
  
### ABOUT
It runs in live boot, so you dont have to install.  
Dislikes Ventoy for some reason.  
Its just a fun think I put together in a few hours, not ment for actual use.  