# How to align full board SVG graphics
- Import graphics at scale 1.0
- `lime.svg`
    - Align RP USB GND pin and Main flash corners with the alignment marks in the SVG
- `aux_*.svg`
    - disable "Fix discontinuities"
    - `aux_logo_*_src.svg` - just as a source before converting the lane dividing stroke and fonts to paths
    - Align the GND pogo pad on USB and GND pad on slider controller
- Double click any part of the SVG and click on the alignment marks to delete them
- Profit
