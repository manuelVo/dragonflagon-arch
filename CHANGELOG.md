# DF Architect

## Release 3.0.7 (2021-10-31)
- FIX: Issue when holding Alt for wall snapping whilc Ctrl is pressed/locked.
- DEV: Migrated to a Webpack/Gulp build chain.

## Release 3.0.6 (2021-10-23)
- FIX: Capture Canvas issue with scene with no background image.

## Release 3.0.5 (2021-10-19)
- FIX: Crash when trying to hide a canvas layer that is not properly registered with FoundryVTT.
- FIX: Crash when attempting to flatten tiles on a scene with no background image.
- FIX: Issue with background colour being transparent by default in FoundryVTT.
- FIX: Ctrl Lock was not being preserved across scene transitions.

## Release 3.0.4 (2021-10-07)
- FIX: Tiles Flattener wasn't excluding hidden tiles properly.
- FIX: Canvas Capture will now hide the borders that appear around hovered and selected Tokens, Tiles, and Drawings.

## Release 3.0.3 (2021-10-05)
- FIX: Counters overlapping due to an error when dismissing them.

## Release 3.0.2 (2021-10-04)
- FIX: _levels undefined when Levels module not installed.
- UPDATE: Spanish Translations courtesy of [lozalojo](https://github.com/lozalojo).

## Release 3.0.1 (2021-09-30)
- FIX: Tile Flattener conflict with the Levels module.
- FIX: Tile Config thumbnail now supports animated tile sources.
- FIX: Object Counter no longer overlaps FPS Meter.
- NEW: Tile Flattener has new option to hide animated tiles.

## Release 3.0.0 (2021-09-29)
- FIX: Quick Colour Picker not invoking the "change" event on the colour selector elements.
- NEW: Including OpenCV library that is only loaded when required.
- UPDATE: Major Optimization in Capture Canvas feature, no longer need to split canvas into many images. This will be done automatically and the resulting images stitched together into a single image download.
- UPDATE: You are now given a prompt for where to save captured image files, either on the server or on your local computer.
- NEW: Introducing a new Canvas Capture API that any module can use.
- NEW: New Tile Flattener feature. This uses the new Canvas Capture API to generate images from the tiles in a quick and efficient way.
- NEW: Tile, Light, Wall, & Sound Counts. Each of these layers will display a small window in the top right of Foundry with the current number of objects in that layer. Hovering the window will display additional information.
- NEW: Toggle the visibility of Walls, Lights, and Sounds controls while on other layers. Simply toggle the Eye button on each layer you want to see.
- NEW: Tile Config now shows a thumbnail of the current image. As well as the width, height, and aspect ratio of the original image.
- NEW: Tile Config now has a scale button beside the width and height. These will use the aspect ratio of the original image to set the width or height depending on which button you press.

## Release 2.1.2 (2021-08-30)
- Fixed broken Wall Chain Lock feature.
- Heavily Improved Wall Chain Lock to no longer require Click+Drag to chain walls. It will now properly immediately auto-chain like Foundry normally does while holding Ctrl.

## Release 2.1.1 (2021-08-27)
- Spanish Localization Update: Courtesy of [lozalojo](https://github.com/lozalojo)

## Release 2.1.0 (2021-08-18)
- Fixed Canvas Capture layer filtering issues when a layer no longer exists.
- Added custom filename field to Canvas Capture dialog.
- Fixed issues with certain wall features that occurred when the currently viewed scene was not the "active" scene.
- Updated Localization files to be in a better hierarchical format.
- Fixed some broken localizations.
- Added check for the Library: DF Hotkeys which is required.
- Update Light Templates to use the new Darkness Range that was introduced in 0.8.x.
- Added a data migration for existing light templates.
- Updated software license from MIT to BSD-3-Clause.

## Release 2.0.2 (2021-06-16)
- Cleaned up some deprecated calls that were flagged in the console.
- Updated the compatibility to FoundryVTT 0.8.7

## Release 2.0.1 (2021-06-06)
- Fixed issue with deleting walls that was introduced with the new wall direction labels.

## Release 2.0.0 (2021-06-06)
- Migrated entire module to FoundryVTT 0.8.6.
- Added Wall direction labels and orientation inversion.
- Added Wall Endpoint Auto-Snapping when dropping a wall with the Alt key held.
- Added Dark Light placement while holding Alt key.
- Now when you have walls selected, you can hold the Ctrl Key while clicking a wall type in the Scene Controls to instantly change the selected walls to that wall type.
- ColorSettings library is now a hard dependency.
- Canvas Capture now preserves the filter and settings selections between uses.
- Fixed Colour Picker so it no longer activates when you hit Enter in a config form.
- Fixed the Capture Canvas so it will no longer deadlock if an exception occurs during the extraction. Also added a warning dialog if the entire canvas is over 100MB in memory size.
- Spanish Localization - Courtesy of [lozalojo](https://github.com/lozalojo)

## Release v1.1.0 (2021-04-18)
- Fixed on-load crash when AltGridSnap is disabled.
- Fixed permission hole where players could switch to GM only layers via the layer hotkeys. Removed the layer hotkeys for non-GMs.
- Added ability to split a canvas render into parts in order to deal with overly large maps that are too big for the GPU.

## Release v1.0.0 (2021-04-09)
- Wall Split/Join: Auto select resulting walls.
- Wall Split/Join: No longer Grid Snapping.
- Canvas Capture: Added layer filtering.
- Canvas Capture: Added option to include padding in the Whole Canvas capture.
- Light Origin: Swapped default colours.
- Light Origin: Correct alignment.
- Added Hotkeys menu to DF Architect settings.
- Light Templates: Macro Directory erroneously adding buttons to sidebar.
- Alt Grid Snap: Added option to move the button from the tools column to the bottom of the controls column.
- Colour Picker: Now generic and API is exposed for other modules to use.
- ReadMe Finally finished!

## Alpha Release v0.9.0 (2021-04-04)
- General code cleanup on light templates.
- Some styling adjustments to the active template dialog.
- You can now create a light template directly from the Macro Directory.
- Standard Light Template Compendiums:
	- Light Templates: D&D5e
	- Light Templates: Pathfinder 1E
	- Light Templates: Pathfinder 2E

## Alpha Release v0.8.0 (2021-04-03)
- Light Templates! You can now create, edit, and place templated lights!

## Alpha Release v0.7.1 (2021-04-03)
- Fixed tile drag+drop issue with Alt Grid snap enabled.

## Alpha Release v0.7.0 (2021-04-02)
- Added canvas image capture. What ever the canvas currently looks like, you can capture that image and save it to a file.

## Alpha Release v0.6.0 (2021-03-29)
- Quick colour picker eyedrop tool for Light Sources.

## Alpha Release v0.5.0 (2021-03-28)
- Added light source crosshairs when holding Shift key.
- Added Bug Reporter integration in manifest.
- Added soft-dependency on "lib - Color Settings".

## Alpha Release v0.4.0 (2021-03-22)
- Added Wall Splitting
- Added Wall Joining

## Alpha Release v0.3.1 (2021-03-15)
- Removed internal Hotkeys implementation.
- Integrated DF Hotkeys library dependency.

## Alpha Release v0.3.0 (2021-03-13)
- Layer Hot Swap shortcut. You can select 2 layers that a hotkey can quickly swap between. Defaulted to `Alt + Q`.
- Added Wall Chain Lock. This essentially inverts the Ctrl key behaviour.
- Added Wall Chain Lock hotkey, defaulted to `Alt + C`.
- Added Wall Type shortcuts. These are defaulted to the keys `Shift + 1` to `Shift + 6`.

## Alpha Release v0.2.0 (2021-03-07)
- Alternate Grid Snapping now works perfectly.
- Added Toggle button to all scene control layers.
- Can be disabled in the module settings (removes the button from the scene controls).

## Alpha Release v0.1.0 (2021-03-07)
- Initial Alpha Release
- Layers now have Hotkeys assigned to quickly switch between them
