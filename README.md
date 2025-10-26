# Sumo Event | SKRIPT

Host exciting, fully server-managed Sumo tournaments! This powerful yet lightweight script transforms your Sumo arena into an automatic elimination system. Players join, and the script handles matches, countdowns, initial freezes, and inventory restoration.



# ✨ Features


Automatic Tournament System: Once started, the script continuously pulls players from the queue until only one winner remains.

Inventory Management: Automatically saves and restores the player's inventory, armor, health, and hunger status upon entry and exit. They won't lose anything! ️

Initial Match Freeze: Locks player movement at the start of a match for a perfect countdown and fair PvP start.

Fall Detection: Automatically eliminates players who fall below a set minimum Y-height.

Custom Knockback: Implements a light, consistent Knockback system for a fun and tactical Sumo PvP experience.

WorldGuard Integration: Recommended support for regions to ensure PvP is only active in the arena.


️# Requirements


 To use this script, you need the following plugins:

Skript (The main plugin to run the script)

Vault (Required for the economy integration/prize money)

WorldGuard (To define the arena )


# Quick Installation

Download and install the required plugins (Skript, SkUtilities, Vault, WorldGuard).

Navigate to your server folder: /plugins/Skript/scripts/

Create a new file named sumo.sk (or any name you prefer) and paste the script code.

Reload Skript in-game or console: /sk reload sumo.sk

If you're an Admin set yourself the permission "sumo.admin"


# ⚙️ Setup and Configuration (Admin Commands)


Before starting the tournament, an administrator must set up 6 essential locations (Permission: sumo.admin).

Command Description
/sumo-setspawn Sets the final return point after the event.
/sumo-setlobby Sets the waiting area/lobby for participants.
/sumo-setpos1 Sets the starting position for Player 1 in the arena.
/sumo-setpos2 Sets the starting position for Player 2 in the arena.
/sumo-setheight Sets the minimum Y-height. Falling below this height eliminates the player.
/sumo-setregion <name> Sets the WorldGuard region (e.g., sumoaregion).
⚠️ WORLDGUARD NOTE: Ensure your Sumo region has the flags: pvp: allow and invincible: deny.



# ▶️ How to Run the Tournament (Automatic Flow)


The tournament runs in just three steps:



1. Start Registration


An Admin starts the event, opening registrations to all players.

/sumo-start

(If the setup is complete, a broadcast will be sent to everyone!)



2. Players Join


Players join the event and are teleported to the waiting lobby.

/sumo-join



3. Start the Automation!


When there are at least 2 players in the queue, an Admin starts the automatic system.

/sumo-startmatches

(The script will take over from here: pulling players, running the countdown, managing wins, and restarting matches until the final winner is declared!)

Player Command Description
/sumo-join Joins the active event.
/sumo-leave Leaves the event and restores inventory.
/sumo-end (Admin) Forces the event to end, restoring all players.

Have fun knocking your opponents off!
