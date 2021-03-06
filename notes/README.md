# CyberBrokers Asset Notes

This sections contains technical notes on CyberBrokers assets and any inconsistencies.

## SVG: Invalid SVG href
<img src="https://raw.githubusercontent.com/CarTarL/CyberBrokers-assets/main/layers/png-render/cb-layer-0065.png" width="100px" style="float: right;"><img src="https://raw.githubusercontent.com/CarTarL/CyberBrokers-assets/main/layers/png-render/cb-layer-0117.png" width="100px" style="float: right;">
   The "triple X backgrounds" have an invalid href link.  This prevents many image utlities from being able to convert from SVG to raster image formats (PNG/JPEG).

**This error has been fixed in all the files in this repository.**  You only need to worry about this if you are pulling SVG files from the contract, metadata, IPFS, OpenSea, etc.

To fix the the issue, one of the following lines from the SVG of the NFT or Layer needs to be removed from the top defs/patterns secction.  Make sure to leave the pattern tag intact - just remove the use tag.

The line you see will depend if the SVG is coming from IPFS, directly from contract, or which background layer is used in the NFT.
- cb-layer-0065, cb-layer-0084, & cb-layer-0117
```
<use xlink:href="#id-bg-6-Group-2">
<use xlink:href="#id-bg-102-Artboard-3">
<use xlink:href="#id-bg-3-Artboard-3">
<use xlink:href="#id-31338">
<use xlink:href="#id-30084">
<use xlink:href="#id-30365">
```

## SVG: missing backgrounds
There are 7 NFTs that have no background
- 688 (Assassin), 1010 (Assassin), 1910 (Gunter), 7585 (Mercenary), 9078 (Gambler), 9510 (Degen), and 9834 (Degen)
