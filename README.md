Sudoku Multiplayer

Installation:
- Create a new Java project
- Delete the App.java file under the src folder (If one was made)
- Place the Client.java, Server.java, and Sudoku.java files into the src folder
- In the terminal while at the root folder of the project, run the command “javac -d bin src/*.java”

For Server Hosting:
- Run the command java -cp bin Server <PORT_NUMBER>.
- Replace <PORT_NUMBER> with the actual port number e.g 8000

For Client Joining:
- Run the command java src/Client.java <PORT_NUMBER> <IPv4_ADDRESS>.
- Replace <PORT_NUMBER> with the actual port number e.g 8000
- If you are joining on a separate device under the same wifi network, put the IPv4 address of the device that is hosting the server. If you are on the same device then you can leave this argument empty.

Controls:
There are 3 commands:
- show: Display the sudoku board
- update [row (0-8), column (0-8), number (0-9)]: Update a spot on the board with its row and column position and the number you want to input.
- quit: If you want to leave the game.

How To Play:
- In Sudoku Multiplayer, the goal is to get the most points by placing the correct numbers in the right spots.
- For every correct placement, you will get one point. You will be told if you place the wrong number.
- The game ends once the entire board is filled up.

Things to Note:
- If all players leave an ongoing game, the server will close.
- When opening the server to other devices, make sure those devices can connect to the server’s IPv4 address. They must be under the same Wifi as the server. You can test this by pinging the server address from your device. If they can’t connect then you might have to edit your server device’s firewall.
