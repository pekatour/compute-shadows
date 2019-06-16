## What is the point of this title pack?
Whenever you want to recalculate shadows from the old versions of ManiaPlanet, or convert Stadium tracks from older Trackmania games, this title pack can do this easily in bulk.

## Why MapType?
This feature was made especially to correctly convert TM1's Platform, Stunt and Puzzle maps to ManiaPlanet, but it can be used in many other ways of course. For example making maps playable if their MapType is lost etc.

## How to use the tool?
First things first, you need to specify the folder where your maps are, relative to Maps/. You can leave it empty to calculate shadows for all maps you have. Next, you can additionally specify MapType which will apply to the calculated maps, or turn this feature off by the little tick button in the corner. Then you're ready to go by clicking Compute Them All.
To terminate the tool, click on the Terminate button in the menu. You have 2 seconds to click on it before another calculation starts. If you're in a calculation process, you can simply click the Back button here (nothing will break by that) and you will be returned to menu to click Terminate. **Note: Shadows will be uncalculated but MapType will still change.**

## How is this better than /calculateallshadows?
You're right, /calculateallshadows does a thing, but you have no control or idea what's being converted.
Before, you also could replicate the same functionality of this tool with few more commands, but since MP4.1, most of these commands broke.

## I've noticed that the map shadows aren't calculated on High, but Default. Why is that?
This was done due to technical things.
If you calculate shadows on higher than Default, the lightmaps aren't saved to the map file, but only to your cache, meaning other people won't see the shadows calculated.
If you want to calculate shadows to highest, I recommend doing it seperately only to maps where you really need them.

## My maps use different MapType than Race. What should I do to keep the original MapType for all the maps?
In the MapType step of the tool, click on the little tick button in the corner. This will turn off the feature.

## I converted a Stadium map from TM1, but several blocks suddently dissapeared. Why?
I'm not exactly sure either, but I consider this as a ManiaPlanet bug, happening especially with sculptures. Same thing would happen if you convert the maps manually.
Currently, I'm trying to find a solution for this. For now, you have no other option to place them manually.