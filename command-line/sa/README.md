# System Administrator's Guide

## Add a New Group

If you want to create a new group on your system, use the groupadd command.

```none
sudo groupadd tpte
```

## Adding a User from the Command Line

In Ubuntu, there are two command-line tools that you can use to create a new user account: `useradd` and `adduser`.

`useradd` is a low-level utility. `adduser` is a script written in Perl that acts as a friendly interactive frontend for `useradd`.

Adding a new user is quick and easy, simply invoke the `adduser` command followed by the username. For example, to create a new user account named `username` you would run:

```none
sudo adduser effie
```

Output:

```none
Adding user `effie' ...
Adding new group `effie' (1002) ...
Adding new user `effie' (1001) with group `effie' ...
Creating home directory `/home/effie' ...
Copying files from `/etc/skel' ...
```

You will be asked a series of questions. Enter and confirm the new user password. Providing an answer to all other questions is optional.

```none
New password: 
Retype new password: 
passwd: password updated successfully
Changing the user information for effie
Enter the new value, or press ENTER for the default
	Full Name []: Efstratia Kazi
	Room Number []: 
	Work Phone []: 
	Home Phone []: 
	Other []: 
Is the information correct? [Y/n] Y
```

## How to Switch Users

It is really simple to switch users in Ubuntu or any other Linux distribution using the terminal.

All you need to do is to know the unsername and its account password and you can switch users with su command:

```none
su effie
```

You’ll be asked to enter the password of the user you want to switch to.

## Add an Existing User Account to a Group

To add an existing user account to a group on your system, use the usermod command, replacing examplegroup with the name of the group you want to add the user to andexampleusername  with the name of the user you want to add.

```none
sudo usermod -a -G tpte effie
```

## How to remove a user from a group

```none
sudo gpasswd -d effie tpte
```

## How to Remove a Group

Groups allow system administrators to apply certain permissions or access to groups of users. It is sometimes necessary to remove a group from a system when it is no longer needed.

Before a group can be removed, any users assigned to the group should be reassigned to another group. To remove a group, you will use the groupdel command.

The syntax for the groupdel command is:

```none
sudo groupdel tpte
```
