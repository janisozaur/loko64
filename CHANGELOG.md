21.02+ (???)
------------------------------------------------------------------------
- Fix: [#294] Crash when setting company name twice.
- Fix: [#794] Game does not stay paused while in construction mode.
- Fix: [#798] Setting waypoints on multitile track/road elements corrupts the position.
- Fix: [#801] Initial save path does not contain a trailing slash.
- Fix: [#807] Incorrect vehicle animation for speed based animations like hydrofoils when at max speed.
- Change: [#787] Scenery and building interaction is now disabled when see-through.

21.02 (2021-02-20)
------------------------------------------------------------------------
- Feature: [#122] Allow vehicles to be cloned from the vehicle window.
- Feature: [#690] Automatically save the game at regular intervals.
- Feature: [#702] Optional new map generator (experimental).
- Fix: [#151] Mouse moves out of window when looking around.
- Fix: [#588] 'Cancel or Show Last Announcement' shortcut doesn't close announcements.
- Fix: [#679] Crash when changing ground texture.
- Fix: [#694] Selecting a song to play is guaranteed to not play it.
- Fix: [#712] Load / save window tries to show preview for item after last.
- Fix: [#721] Incorrect catchment area for airports.
- Fix: [#725] Company value graph does not display correctly.
- Fix: [#744] Rendering issues ('Z-fighting') with vehicles over bridges.
- Fix: [#766] Performance index is off by a factor of 10 in scenario options window.
- Fix: [#769] Waypoints for road vehicles could not be set.
- Fix: [#779] Town list displays the wrong amount of stations.
- Change: [#690] Default saved game directory is now in OpenLoco user directory.
- Change: [#762] The vehicle window now uses buttons for local/express mode.

20.10 (2020-10-25)
------------------------------------------------------------------------
- Feature: [#569] Option/cheat to disable AI companies entirely.
- Fix: [#573] Crash caused by opening Road construction window.
- Fix: [#588] Crash caused by changing default audio device.
- Fix: [#595] Implementation mistake in CreateVehicle could lead to crashes.
- Fix: [#635] Land tool not working properly, due to tool drag events not passing on coordinates.
- Fix: [#648] Fix crash in vehicle update head caused by CreateVehicle.

20.07 (2020-07-26)
------------------------------------------------------------------------
- Feature: [#523] Holding the construction window's build or remove button will keep repeating the action.
- Fix: [#158] Pressing shift to build underground tracks automatically builds ten track pieces.
- Fix: [#390] Load/save window causes a crash when trying to access bad directories.
- Fix: [#397] Opening a tutorial crashes the game.
- Fix: [#485] Incorrect position of exhaust smoke on vehicles.
- Fix: [#491] Station/city name labels are hidden from viewport when saving.
- Fix: [#529] Tree-related industries are not updating properly.
- Fix: [#530] Industry production not starting up under some conditions.
- Removed: Clicking track / road construction while holding shift will place 10 pieces in a row.

20.05.1 (2020-05-30)
------------------------------------------------------------------------
- Fix: [#487] Checkbox behaviour reversed for industry opening/closing in landscape generation options.
- Fix: [#488] Repeated clicking may lead to a negative loan.
- Fix: [#494] Farms not producing grain for stations in Mountain Mayhem scenario.
- Fix: [#498] Clicking newly invented vehicle in news throws out of range exception.

20.05 (2020-05-24)
------------------------------------------------------------------------
- Feature: [#77] Add "Exit OpenLoco" to the main menu.
- Fix: [#264] Option 'Export plug-in objects with saved games' is partially cut off.
- Fix: [#299, #430] Crash due to added null-chars when manually specifying Locomotion directory.
- Fix: [#359] Widgets tied to tools could get stuck in pressed state.
- Fix: [#388] Re-center Options window on scale factor change.
- Fix: [#396] Preferred owner name is not saved.
- Fix: [#409] Incorrect refund cost when deleting signals.
- Fix: [#412] Game crashes after a while on Great Britain & Ireland 1930.
- Fix: [#423] Date in challenge tooltip is incorrect.
- Fix: [#425] Changing resolution in fullscreen mode doesn't work.
- Fix: [#428] Show an error when a vehicle can't be built due to invalid properties. (Original bug.)
- Fix: [#440] Final segment in town population graphs could show no population.
- Fix: [#467] Incorrect scrolling thumbs when leaving the bottom of an auto resizing window.
- Fix: [#478] Crash when opening narrow gauge tab on train purchasing window
- Change: [#420] Disable window scale factor buttons when not applicable.

20.03 (2020-03-23)
------------------------------------------------------------------------
- Feature: [#347] Screenshots are now saved in PNG format.
- Fix: [#226] Zooming to cursor is buggy on bigger maps.
- Fix: [#296] Correctly show challenge progression in save previews.
- Fix: [#297] Menu click sound not played.
- Fix: [#303] Play title music preference is not saved.
- Fix: [#340] Cargo rating is calculated incorrectly in some edge cases.
- Fix: [#349] Building a signal adds money (macOS/Linux only).
- Fix: [#383] Crash in construction window.
- Fix: Strings were not wrapping properly in the file browser window.
- Change: [#380] Make keypad enter work the same as normal enter.

19.03 (2019-03-01)
------------------------------------------------------------------------
- Feature: [#163] Remove terraforming limits outside of scenario editor.
- Feature: [#178] Allow zooming to cursor position instead of viewport centre.
- Feature: [#192] The option window now includes OpenLoco-specific settings.
- Feature: [#203] Support multiple languages by loading text strings from YAML files.
- Feature: [#212] Add fullscreen support.
- Feature: [#221, #236] Implement audio through SDL2 mixer, introducing audio on Linux and macOS.
- Feature: [#237] Allow nearest neighbour scaling the game on integer intervals.
- Feature: [#275] Allow disabling the title screen music.
- Feature: [#279] Use OpenLoco logo for window icon. (Logo created by [Zcooger](https://github.com/Zcooger))
- Fix: Tooltips were calling the wrong event.
- Fix: [#219, #257] Prevent text from being drawn off-screen.
- Change: [#107] Show git branch and short sha1 hash in version info line.
- Change: [#211] Store configuration file as YAML.

18.02 (2018-02-15)
------------------------------------------------------------------------
- Feature: [#12, #14, #50] Support for Linux and macOS.
- Feature: [#20] Support graphics data files from Stream distribution.
- Feature: Allow player to remove roads that are in use.
- Feature: Towns can now always be renamed (As seen in OpenTTD).
- Feature: Vehicle breakdowns can now be disabled (As seen in OpenTTD).
- Feature: Playable in a resizable window.
- Feature: Clicking track / road construction while holding shift will place 10 pieces in a row.
- Change: [#79] Store `game.cfg`, `plugin.dat` and `scores.dat` in:
  - Windows: `%APPDATA%\OpenLoco`
  - Linux: `~/.config/openloco`
  - macOS: `~/Library/Application Support/OpenLoco`
- Change: [#79] Disable file existence and size checks.
