# **Chess Game**
Simple network chess game created with C

## Sketch
<img src="https://user-images.githubusercontent.com/48203569/100318194-feecd800-3000-11eb-9ed5-92cfc6788dd9.jpg" width="850" height="600">
                                                                                                                                     
## Features
  * Used [epoll](https://en.wikipedia.org/wiki/Epoll) for accepting 2 clients
  * Control this game with a keyboard only
  * Used unicode \u2654 ~ \u265F for the pieces
  * Promotion  
  * Quit
  
## Usage
* Server
  ```
  gcc server.c -o server
  ./server <PORT>
  ```
    
* Client
  ```
  gcc client.c -o client -lpthread -lncursesw
  ./client <IP> <PORT>
  ```
  
 * Move a piece  
  1. Control the cursor with Keyboard arrow keys and press **ENTER** on a your piece you want to move.
  2. Move the cursor to the location where you want to move the piece and press **ENTER**.

## Demo
<img src="https://user-images.githubusercontent.com/48203569/100316691-65bcc200-2ffe-11eb-8c05-adcfa16f2cf6.gif" width="850" height="600">

## Library used
* [ncurses](https://invisible-island.net/ncurses/announce.html)
