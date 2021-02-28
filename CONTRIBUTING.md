# How to contribute your mod to this database:
### 1. In the top right, select "Fork" and fork the repository to your own account. After a bit you will be redirected to your fork.
![Figure 1](https://i.imgur.com/mAirFMb.png)

### 2. Click into the category folder that you want to place your mod in.
![Figure 2](https://i.imgur.com/MPN53rv.png)

### 3. In the top right, click "Add file" then select "Create new file".
![Figure 3](https://i.imgur.com/CFX5QYm.png)

### 4. Type your mod's GUID (unique identifier, generally `SomethingLikeThis` using only alpha-numeric characters) then a slash (`/`), then the version number of your mod followed by `.json`. Example: `MyExampleMod/0.5.2.json`
![Figure 4](https://i.imgur.com/9drVvYu.png)

### 5. Copy the template mod entry from below and paste it into the editing area. Proceed to fill out all the fields, using other existing mods as a reference if needed. More information on the install steps and dependencies can be found below too.
```JSON
{
	"Name": "Your Mod Name",
	"VersionNumber": "1.0.0",
	"Description": "Your mod's description. This appears on the sidebar!",
	"ShortDescription": "A short description that appears on the mod's card in the list",
	"Authors": ["Your name", "Maybe another author"],
	"IconUrl": "URL to the icon you want to use for your mod",
	"SourceUrl": "URL to a GitHub or BoneTome page",
	"DownloadUrl": "Download URL of your mod",
	"InstallationSteps": [
		"extract $GAME_DIR"
	],
	"Dependencies": {
		"BepInEx": "^5.4.5",
		"Deli": "~0.2.5"
	}
}
```

Install Steps:
* `extract [location]`: extracts the downloaded archive to the folder specified. Example: `extract $GAME_DIR/VirtualObjects`
* `move [location]`: Moves the downloaded file to the specified location. Example: `move mods/MyMod_0.2.5.deli`

Dependencies are standard semantic version ranges. Place the GUID of the mod you need to install before yours on the left and then the required version number on the right.
Generally you want to prefix the version number with a `^`.
More complex rules can be found here: https://devhints.io/semver

### 6. Once you're done filling out the information, scroll to the bottom and commit your changes (keeping the 'commit directly to main' option selected)
![Figure 5](https://i.imgur.com/ST08ThJ.png)

### 7. Return to the main page of your fork by clicking on the name in the top left
![Figure 6](https://i.imgur.com/GA1wIi1.png)

### 8. After commiting this new file, there is now a new option to create a pull request back into the main repository. Click the new button and then the green "create pull request" button on the following page.
![Figure 7](https://i.imgur.com/Nx22QGv.png)

### 9. Enter some details about the file you've just added (your name, your mods's name) and then create the pull request.
![Figure 8](https://i.imgur.com/tD9hG7q.png)

### 10. The request will be reviewed by someone with permissions and when it is accepted (merged) your mod will have been added to the database!
