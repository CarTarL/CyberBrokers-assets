# CyberBrokers Layers

Each NFT is a unique collecton of SVG layers, that are ordered properly, and then combined into a single SVG file.

Each folders contains image files in the format: cb-layer-XXXX.EXT where XXXX is ID of the layer, zero padded to 4 digits, and EXT is the file format extensions like png or svg.

There have been a couple of modifications to these files from what is found in the contract. See the Notes section for details.

## Original SVG layers
- svg-render directory
- The individual layers only exist on-chain.  
- They have been retrieved from the contract and turned into individual SVG files.
- Id tags are numbers, to save space.  There is no individual source of layers with Id tags as text descriptors.
- The width/height of these files match the NFT files, and layers are properly positioned for stacking layers.

## Modified SVG layers
- svg-unbound directory
- Individual layers that are unbound from the full width/height of the broker bounding box.
- The width/height matches the exact size of the layer itself, with no margin.
- These are more useful for displaying multiple layers on a single page as it saves space.
- There were created from the svg-render version using the Inkspace command: 
  ```inkscape --export-area-drawing```

## PNG versions
PNG versions of all the above are also provided. These are rendered at the same resolution as the SVG version.  See NFT directory for best tools to convert from SVG to PNG, JPEG, or other raster formats.

## Zip files
If you need to download all layers of a given format at once, they are Zip files in the zip directory.

**For PNG versions it would be appreciated if you download the corresponding SVG Zip file and uand then use a tool locally to create the PNG versions.** This will help keep this repository in place and not cost me a fortune !
