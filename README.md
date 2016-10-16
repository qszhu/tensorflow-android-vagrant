Note: required to download various packages when building, please ensure a good network connection before continuing.

### 1. Setup virtual machine
* Download and install [Vagrant](https://www.vagrantup.com/downloads.html)
* Download and install [VirtualBox](https://www.virtualbox.org/)
* Install [Ansible](http://docs.ansible.com/ansible/intro_installation.html), e.g. `pip install ansible`

### 2. Prepare virtual machine environment
* In the command line, run:
```bash
$ ./setup
```

### 3. Start the virtual machine
* Optional: adjust the vm memory and cpu settings in the `Vagrantfile` accordingly
* In the command line, run:
```bash
$ vagrant up
```

### 4. Build the android app
```bash
$ ./build
```

The output apk file will be put at `ansible/downloads`
