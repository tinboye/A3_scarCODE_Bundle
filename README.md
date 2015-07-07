# ArmA 3 ScarCode Scripts Bundle by IT07
Hi and thanks for checking out this repository.<br />
It is important to note that all of the script below are designed for ArmA 3 Epoch mod.<br />
Small structural changes need to be applied to get them working for a different mod however that is not the purpose of these scripts.<br />

#### Contents of this repository
- ArmA 3 Anti-PvP (PvE) <br />
- ScarCode Menu Package (S.C.M.P.) <br />
- Player Support Requester menu (P.S.R.) <br />
- Server Restart Warnings (S.R.W.) <br />
- Server Info Menu (S.I.M.) <br />
- Server Intro Credits (introCredits) <br />
- Server Intro Camera (introCam) <br />
- Spawn Teleport Menu (S.T.M.) <br />
- Simple Ammo Repacker (S.A.R) <br />

#### Quick install instructions
- if you install anyting that uses a scrollmenu and you have infiSTAR, make sure things in infiSTARsettings.txt match yours <br />
- any scarCODE menu needs the `#include "scarCODE\global.hpp"` file included in description.ext. Check the description.ext example in this repository to see how to do so.
- PVE/anti-PVP script needs *a3_scarCODE_PVE* in *@epochhive\addons* <br />
- PSR script needs *a3_scarCODE_PSR* in *@epochhive\addons* <br />
**Make sure to repack the contents of the server-side folder into a pbo named exactly the same as the folder they came in**

#### Extended installation instructions
I will try to keep this as short as possible because explaining how to install it (with the idea in mind that the reader does not already know how to) is very hard. It is like explaining to someone how to build a car but that someone does not know anything about cars. Allright here we go:<br />
- None of these scripts use ExecVM to start them. It is all inside functions that use `postInit = 1` because that will make it so ArmA automatically executes the function upon game start.<br />
- Check the `description.ext (example)` and look at how it has been written. It should give you more light on how to do all of this. Add the lines you need to your own description.ext to get it working of course :) <br />
- `description.ext (example)` has all the code you need for your own description.ext to get the scripts to work you want to use. Make sure you only copy the code you want. More examples coming soon.

#### Additional info
- If you want to use PvE/Anti-PvP script, you will need to place onPlayerKilled.sqf in the root of your missionfile.<br />

#### Config file locations
**PSR:** `scarCODE\PSR\config_PSR.hpp` and `a3_scarCODE_PSR\putUIDsInHere.sqf` <br />
**PVE:** `scarCODE\PVE\fn_initPVE.sqf` <br />
**SCMP:** `scarCODE\SCMP\config_SCMP.hpp` <br />
**SIM:** `scarCODE\SIM\config_SIM.hpp` <br />
**SRW:** `scarCODE\SRW\config.sqf` <br />
**STM:** `scarCODE\STM\config_STM` <br />
**Also do not forget to read the comments in the example description.ext as it describes vital info on getting this all to work**

#### BattlEye Filters
I recommend getting a good antihack like http://infistar.de and then remove your scripts.txt.
It improves performance and saves you a lot of frustration from all those kicks. Also, the really advanced "hackers" usually have a bypass or they use command that are covered by the rest of the filters.
