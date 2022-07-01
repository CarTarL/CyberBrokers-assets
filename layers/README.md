# CyberBrokers Layers

Each NFT is a unique collecton of SVG layers, that are ordered properly, and then combined into a single SVG file.

Each folders contains image files in the format: cb-layer-XXXX.EXT where XXXX is ID of the layer, zero padded to 4 digits, and EXT is the file format extensions like png or svg.

There have been a couple of modifications to these files from what is found in the contract. See the Notes section for details.

## svg-render
- The individual layers only exist on-chain.  
- They have been retrieved from the contract and turned into individual SVG files.
- Id tags are numbers, to save space.  There is no individual source of layers with Id tags as text descriptors.
- The x/y dimensions of these files match the NFT files, and layers are properly positioned for stacking layers.

## svg-unbound
- 
