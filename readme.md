# WD vragrant 

## Description

Vagrant configuration used in WD context

## Usage 

- Go to the project path's folder and start the vagrant box : 
```
git clone https://github.com/vs-webdrone/WD_vagrant.git
cd $(basename "WD_vagrant" .git)
vagrant up
```

- Connect to the vagrant box, to (manually) check that everything is ok :
```
vagrant ssh
```

- Finally destroy the box, when all the (manual) check are done :
```
vagrant destroy
```

## troubleshooting 

- Set the vagrant's log level :
```
set VAGRANT_LOG=info
```


## source :

- [Vagrant debug documentation](https://developer.hashicorp.com/vagrant/docs/other/debugging)
- [10 basic vagrant cmd](https://medium.com/@shaik.imp/vagrant-commands-for-vm-life-cycle-management-e11c3167638e)