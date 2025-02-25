# CWC_SimpleGantt

## A very simple Custom Web Control (CWC) to create a Gantt chart with chart.js in WinCC Unified

![Gantt Chart]({867a58d6-397f-47c1-94ae-82207ddc773b}/assets/learning.png)

Icon created by [Jagat Icon - Flaticon](https://www.flaticon.com/free-icons/gantt")

Based on [chartJS](https://chartjs.org).

## ToDo:

- [x] Get request by customers
- [x] Find a timeslot
- [x] Write code
- [x] Debug
- [ ] Write documentation

## How to create a CWC from this stuff:

1. Download/pull/whatever the code
2. cd in the **{867a58d6-397f-47c1-94ae-82207ddc773b}** folder
3. Create **{867a58d6-397f-47c1-94ae-82207ddc773b}.zip** file with the **{867a58d6-397f-47c1-94ae-82207ddc773b}** folder content
> [!IMPORTANT]
> Do not include the **{867a58d6-397f-47c1-94ae-82207ddc773b}** folder itself as root folder in the file zip!
4. Copy the **{867a58d6-397f-47c1-94ae-82207ddc773b}.zip** file in **C:\Program Files\Siemens\Automation\Portal V1x\Data\Hmi\CustomControls** folder
5. Refresh the **My Controls** right side pane in the TIA Portal WinCC Unified screen editor
6. Enjoy

## How to directly download this CWC (if you are in a hurry):
1. Download from [here](build/{867a58d6-397f-47c1-94ae-82207ddc773b}.zip)
2. Copy the **{867a58d6-397f-47c1-94ae-82207ddc773b}.zip** file in **C:\Program Files\Siemens\Automation\Portal Vxx\Data\Hmi\CustomControls** folder
3. Refresh the **My Controls** right side pane in the TIA Portal WinCC Unified screen editor
4. Enjoy


## Documentation:

### How to use this?
This CWC (Custom Web Control) exposes several parameters (see the [manifest file]({867a58d6-397f-47c1-94ae-82207ddc773b}/manifest.json) for details). All of them are dynamic, so you can assign static values in TIA Portal or dynamize them connecting tags, scripts, etc...

Every Gantt phase is composed by 3 sub-phases ("golden", "last" and "actual"). 

#### Phases
A TIA Portal empty array you can populate with how much phases as you want. For each phase you have to define the beginning time and the duration of the golden, the last and the actual phase.

#### ColorGolden
A TIA Portal color object (Alpha, R, G, B) which is used to plot all the "golden" sub-phases.

#### ColorLast
A TIA Portal color object (Alpha, R, G, B) which is used to plot all the "last" sub-phases.

#### ColorActual
A TIA Portal color object (Alpha, R, G, B) which is used to plot all the "actual" sub-phases.

This CWC exposes a method too:

#### ForceRedraw
This just calls an update method on the chartJS object, with current configuration and dataset.

## May I ask for support on this CWC?
Sure: just drop me an [email](mailto:marco.buffa@siemens.com).
