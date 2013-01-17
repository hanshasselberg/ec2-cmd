# ec2-cmd

its a tool to show servers and execute commands on them.

## Installation

```
gem install thor term-ansicolor
git clone https://github.com/i0rek/ec2-cmd.git
cd ec2-cmd
ln - ln -fs `pwd`/ec2-cmd /usr/local/bin/ec2-cmd
```

## Usage

Show beta servers:

```
$ ec2-cmd do bouncer
PGBouncer_1
PGBouncer_2
PGBouncer_3
PGBouncer_4
```

Execute a command on all of them:

```
$ ec2-cmd do bouncer "pwd"
PGBouncer_1: /home/ubuntu
PGBouncer_2: /home/ubuntu
PGBouncer_3: /home/ubuntu
PGBouncer_4: /home/ubuntu
```
