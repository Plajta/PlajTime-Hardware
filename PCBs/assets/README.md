# PlajTime PCB Assets
- `source files` - contains sources for further editing - state before converting broken things and fonts to paths
    - if you apply these directly to KiCAD text won't render and it will be EXTREMELY laggy because of KiCADs bad curve calculations
- For some text we used the awesome ISO style font [osifont](https://github.com/hikikomori82/osifont)
- For new boards we use the `Space Grotesk` and `Syncopate` Google Fonts
- To get the appliable graphics from the source ones you need to:
    1) Ungroup everything (Ctrl+Shift+G)
    2) Run `Path -> Stroke to Path` on everything
    3) Transform (`Object -> Transform...`) everything proportionally by 1000% using `Scale`
    4) Apply `Extensions -> Modify Path -> Approximate Curves by Straight lines` with 0,1 (or more if you don't mind losing detail)
    5) Transform (`Object -> Transform...`) everything proportionally by 10% using `Scale`

## How to align full board SVG graphics
- open the import graphics menu
- disable "Fix discontinuities"
- set scale to 1.0
- `lime.svg`
    - Align RP USB GND pin and Main flash corners with the alignment marks in the SVG
- `aux_*.svg`
    - Align the GND pogo pad on USB and GND pad on slider controller
- `bat_*.svg`
    - Align the two vias to GND and BATT_NTC
- `charger_*.svg`
    - Align edge cuts
- Double click any part of the SVG and click on the alignment marks to delete them
- Profit
