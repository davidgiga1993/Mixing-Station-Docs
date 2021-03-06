# Actions

Actions are used to assign a parameter or app functionality to a custom button/knob or midi controller.

## Action types
Depending on the current mixer type more or less action types are available.

- Channel based actions
  - Current channel: Actions for the currently selected channel
  - Current layer: Actions for the channels inside the current layer
  - Fixed channel: Actions for a fixed channel
- FX: Actions for the FX racks
- Mutegroup
- Open view: Opens a view
- Layer based actions
- Sends on fader: Activates/Deactivates sends on fader
- Select Layer: Selects a layer
- ...

## Channel based actions
These actions can be used to change a value of a channel

- Current channel: Values of the last opened channel can be changed
- Current layer: Values of any channel in the current layer can be changed. Use the "Channel offset" parameter to select which channel of the current layer should be used (1 is the channel on the left).
- Fixed channel: Changes a value of a fixed channel


### Settings: Invert output
The `Invert output` button can be used to invert the output. This might be useful when you want to create a mute button, but the channel only got a "on" function.

### Settings: Use SoF
When activated the `Fader`, `Pan`, `On` values will be affected by sends on fader. When this is disabled these values will always only affect the main mix.

## FX
Allows FX value changes. This action also has tap delay support for the `time` value of an FX.


## Mutegroup
Changes the status of a mutegroup

## Open view
Opens a view in the app. Depending on the mixer more or less views are available. 
**Note:** No other actions in the list will be executed after this action. If you want for example to change a layer and open a view, place the "open view" action last.

## Sends on fader
Changes the current sends on fader status and target mix.


## Show
The show action can load cues, scenes or other show related stuff.
Depending on the current mixer the available actions might change.

### XM32
- Current: Does nothing but has the value of the currently loaded show item.
- Go: Loads the item selected as `next`. Has the name of the next item as value
- Next: Moved the `next` selection to the next item. Has the same value as `Go`
- Go+Next: Executes `Go` and then `Next`
- Prev: Moves the "next" selection one item back.
- Go+Prev: Executes `Go` and then `Prev`
- Load x: Loads the item as position X