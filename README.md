Environment installation

You will need few things to start with since the whole environment is prepared in Vagrant

Install VirtualBox https://www.virtualbox.org/wiki/Downloads

Install Vagrant https://www.vagrantup.com/downloads.html

Install VBGuest plugin for folder syncing by running
```  
  vagrant plugin install vagrant-vbguest
```

Afterwards you can go ahead and spin-up the VM itself.
```
  cd <path to the clone of this repository>
  vagrant up
```
