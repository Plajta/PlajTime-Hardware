# PlajTime PCB Assets
- `source files` - contains sources for further editing - state before converting broken things and fonts to paths
- For some text we used the awesome ISO style font [osifont](https://github.com/hikikomori82/osifont)

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
- Double click any part of the SVG and click on the alignment marks to delete them
- Profit
