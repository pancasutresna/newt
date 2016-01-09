# newt
Basic NodeJS development vagrant box with MongoDB and Redis Installed

### What's in the box?
- Ubuntu (14.04)
- NodeJS
- MongoDB
- Redis


Clone this repository, then run
```
vagrant up --provider=virtualbox
```

Or you could just use preconfigured box using this command:
```
vagrant init panca_sutresna/newt; vagrant up --provider virtualbox
```

### Notes
Change forwarded_port option to your desired port:
Open Vagrantfile, change line 25 to
 ```
config.vm.network "forwarded_port", guest: [your desired port], host: [your desired port]
```
default is 4000.

Thanks,
