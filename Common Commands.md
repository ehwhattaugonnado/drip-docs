
# Common Commands
Open the server that you need in dathost and go to the console tab. All commands will be entered there.
## Force Start Match
`css_start`Will skip the readying and immediately start the match. If knife round is enable it will go to the knife round. 
## Force End Match
`css_endmatch` Immediately ends the match
## Reload Round
`css_stop` If the round is live this will stop the round and restore a backup of the previous round  
`css_restore <Round Number>` Will restore the specified round number  
For more complex scenarios see [Loading a Backup](<Loading%20a%20Backup.md>)

## Change Map
`css_map <de_map>` Ensure you enter the entire map name ie `de_ancient`. You can also enter a workshop map id and it will load.  
`css_rmap` to reload the current map
## Pause
These are the MatchZy pause and unpause commands.   
`css_forcepause`  or `css_fp`   
`css_forceunpause` or `css_fup`
## Toggle Knife round
`css_roundknife` of `css_rk` This will toggle the status of the knife round and should output to console `"Knife round is now {knifeStatus}!"`
## Toggle Playout/Max Rounds
`css_playout` This will allow teams to play a full 24 rounds for scrim purposes. 