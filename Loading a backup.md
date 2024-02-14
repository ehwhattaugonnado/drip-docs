# How to reload a round:  
Players can reload a round in the server themselves. \
[`.stop`](https://shobhit-pathak.github.io/MatchZy/commands/) Restore the backup of the current round (Both teams need to type .stop to restore the current round)
1. Reloading the previous round:  
	-   [`mp_backup_round_file_last`](https://totalcsgo.com/commands/mpbackuproundfilelast) This will give you the filename for the most recent round in the console
	-   [`mp_backup_restore_load_file <Backup File> `](https://totalcsgo.com/commands/mpbackuprestoreloadfile) Replace <Backup File> with the filename that was the output of the previous command
2. Reloading a specific previous round
	-   [`mp_backup_restore_list_files <Limit> `](https://totalcsgo.com/commands/mpbackuprestorelistfiles) Limit will set the number of rounds for it to look back. If no limit is given it will list all round
	-   [`mp_backup_restore_load_file <Backup File> `](https://totalcsgo.com/commands/mpbackuprestoreloadfile) Replace <Backup File> with the filename that was the output of the previous command
3. Restoring the round on a new server
	- Find the filename of the round that needs to be restored using one of the previous commands.
	- Go to the File Manager. Find the name of the file, these will be in the root cs2 folder (just scroll down, don’t open any folders). Right click -> Download file
	- Boot a copy of the scrim server template. In file manager drag the downloaded file into the root cs2 directory
	- Have everyone connect and join the correct team.
	- Run the backup restore round command once everyone is connected and on the correct team