# TCP-UDP-Chat
A chat where people can talk together wether they use a TCP or a UDP protocols. Made to demonstrate difference between TCP and UDP.
Uses ncurses library.

## Usage

### Install ncurses

```bash
sudo apt remove libncurses5-dev libncursesw5-dev
```

### Uninstall ncurses

```bash
sudo apt remove libncurses5-dev libncursesw5-dev
```

### Compilation

#### Client

```bash
gcc client.c -o client -lcurses
```

#### Server

```bash
gcc serveur.c -o serveur
```

### Execution

#### Client

```bash
./client <arguments>
``` 

Arguments :
|Argument|Description|Required|Default|
|------------|------------|------------|------------|
|-i|ipv4 server address|Yes||
|-l|Username|Yes||
|-p|Server port|Yes||
|-t|Use TCP|Yes||
|-u|Use UDP|Yes||

#### Server

```bash
./serveur <arguments>
``` 

Arguments :
|Argument|Description|Required|Default|
|------------|------------|------------|------------|
|-m|Maximum cients at the same time|No|100|
|-p|Listening port|No|2021|

### Close program

Use `/quit` to leave chat.
