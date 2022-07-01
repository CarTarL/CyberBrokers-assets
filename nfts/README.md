# CyberBrokers NFTs

This section contains all 10,001 NFTs in various image formats and configurations.

Each folders contains image files in the format: cb-XXXXX.EXT where XXXXX is the token id of the NFT, zero padded to 5 digits, and EXT is the file format extensions like png or svg.

There have been a couple of modifications to these files from what is found on IPFS or in the contract.  See the Notes section for details.

The original SVG files from CyberBrokers are contained in these folders.
- svg-ipfs - These are the SVG files on IPFS and  referenced in the metadata.  Id tags are text descriptors.
- svg-render - These come directly from contract rendering.  Id tags are numbers, to save space.

Other than the different in id tag format, both of these are identical version of the NFTs.  The svg-render version may be more useful for those that want to turn on/off layers of a given NFT in an application, as the contract provides id tags in numbers, not text descriptors.

The following additional formats are provided for ease of use.
- svg-nb - The NFTs without their background image.
- svg-card - The NFTs overlayed with a Broker Card, providing metadata information in a single image.

PNG versions of all the above are also provided.  These are rendered at the same resolution as the SVG version.

Not all tools do a good job of converting SVG to PNG, JPG, or any raster format.  I recommend the following tools for converting the SVG NFTs into other formats like PNG or JPEG.  You can also use these tools to increase/descrease resolution at the SVG level and then convert to image formats, keeping the best resolution possible. 
- Windows - [Inkscape](https://inkscape.org/) has a user interface you can use to pull apart layers and a command line utility to convert multiple files at a single time.
- Linux: [rsvg-convert](https://wiki.gnome.org/action/show/Projects/LibRsvg?action=show&redirect=LibRsvg) is part of the librsvg package available on most linux varients and can be installed with apt or yum.  It is a command line utility with lots of options as well.

If you need to download all 10,001 NFTs of a given format at once, they are Zip files in the zip directory.

**For PNG versions it would be appreciated if you download the corresponding SVG Zip file and uand then use a tool locally to create the PNG versions.**  
This will help keep this repository in place and not cost me a fortune !
