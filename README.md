# Sparta Node App

## Download

git clone https://github.com/Maksaud/app-starter-code-exercise.git

## Summary
This is a node js app made by sparta that have different pages that run on development.local:
- Fibonacce
- blog
- hack

### Prerequisites
- Github
- Virutal box:
  - Where to find virtual box:  https://www.virtualbox.org/ and click download
- Vagrant box:
  - Where to find virtual box:  https://www.vagrantup.com/downloads.html, Chose the OS and then  click download
- Vagrant host updater
- ruby
- rails
- rake

### Virtual Machine and Vagrant

Virtual machine
- A virtual machine behaves like a seperate computer with virtual hardware. It runs as a process on your machine.
- The tool used for createing a virtual machine for this app will be virtual box

Vagrant
- Vagrant is a tool that allows you to build and maintain environments.

#### To set up a virtualised environment and to test if the app is going to work

The Vagrantfile is configured so that there will be 2 virtual machines:
- Machine for the node App
- Machine for the databse

First go onto the tests directory then run this command

```
rake spec
```

Make sure you have Vagrant and virtual box installed on your device and you are in the same directory of the Vagrantfile.

To test if the virtual machines are correctly provisioned:

To run create, start and provision the virtual machine

```
vagrant up
```

The vagrant up will create, start and provision the app and the database.

to do them seperately you will have to specify the name of the machine you want to create:

```
vagrant up app
```
or
```
vagrant up db
```

To enter the virtual machine use:

```
vagrant ssh <name of machine>
```

the name of the machine can either be db or app

### To test the app

Make sure you are in the virtual machine so that you are in the environment where the requirements for the app and database are installed.

First go inside the app directory inside the repository

then run this command
```
npm test
```

### To run the node app

First go into the app directory inside the repository.

Then run this command
```
npm start
```

### How to view the app

To view the app you must first make sure it is running and make sure it is listening on port 3000 (It should tell you on the terminal)

Then type *development.local/* onto your browser

#### Fibonacce

Make sure your app is running

Then type in the url *development.local/fibonacce/<any number>*

#### Post

Make sure your app is running

Then type in the url *development.local/posts*

#### Hack

Make sure your app is running

Then type in the url *development.local/hack <script>*
