# NBAuth
License system for NicolasBrg's products.
With the new system, keep an eye on your updates, connections and licenses, track the history of disconnections and enjoy better activity tracking in case of problems, with improved debugging and a built-in solution to avoid disconnections.

Managing mods and their web APIs has never been easier for you.

## Quick to use
When you get a license, you will receive several information, here is an example:
```json
{
    "Name": "NAME",
    "Key": "KEY",
    "Product": "PRODUCT",
    "VerificationData": "",
    "LastRaw": "",
    "Version": "",
    "LastConnexion": "",
    "Down": {

    }
}
```
With a pre-made command with this syntax: 
```
/nbauth_PRODUCT connect NAME KEY
```
You just have to execute the generated command.

## Permissions
To use the authentication system you must have the permission: 
```
nbauth.admin
```
 
## Advanced
### Commands
/nbauth_PRODUCT <Action?> <Arg_1?> <Arg_2?>
- connect <Name?> <Key?>
  - If the name and the key are given they are defined and a connection attempt is run, otherwise a connection attempt start.
- name <Name?>
  - Defines the name of the server / network if the argument is given, otherwise it is displayed.
- key <Key>
  - Defines the license key of the server / network if the argument is given.
- type
  - Displays the type of license connected (Unknown / Simple / Network / Private).
- product: 
  - Displays product information.
- last_connexion: 
  - Displays the last connexion.
- debug: 
  - Displays all the information needed to debug the license, take the reflex to send a screenshot of this when you send a bug report or encounter a problem.
- version: 
  - Displays the installed version of the product.
- down: 
  - Displays the number of disconnections to the server and the corresponding errors.
- clear_down
  - Removes the list of downs from the server.

#### Example
Starts a connection attempt for NBTeams.
```
/nbauth_nbteams connect
```
Set the server name to TEST into NBTeams
```
/nbauth_nbteams name TEST
```
Display debug information for NBStatues
```
/nbauth_nbstatues debug
```

### General operation
When creating your license, the IPs linked to your server are automatically registered for 2 to 4 days, after this time, the addresses will have to be added manually on the online interface (if you have the access) or by asking NicolasBrg.

IP addresses have several status, including:
- Pending
- Validated
- Suspended
- Banned

### Getting help
To get help it's very simple, just use the debug command, inspect the result, if you don't understand, contact NicolasBrg or look on your online interface if you got the access

### Web Interface
Here is a preview of the online interface allowing you to follow your licenses, this one is currently in BETA, all rights reserved. If you want to get access to the platform, contact NicolasBrg.

![image](https://user-images.githubusercontent.com/30299182/177173668-aedf39bf-8ae4-4226-a114-8f936e3c820e.png)
![image](https://user-images.githubusercontent.com/30299182/177173958-ebe55e28-b7f6-4f6d-8022-9b7ff0d2e01a.png)
![image](https://user-images.githubusercontent.com/30299182/177174092-aaa6d90b-1744-4760-9145-b32b6d1a02be.png)

## Compatible products
NBTeams, NBStatues, NBMacro, NBGames, NBTreasureChest
