# CyberBrokers NFTs

This section contains all 10,001 NFTs in various image formats and configurations.

Each folders contains image files in the format: cb-XXXXX.EXT where XXXXX is the token id of the NFT, zero padded to 5 digits, and EXT is the file format extensions like png or svg.

There have been a couple of modifications to these files from what is found on IPFS or in the contract.  See the Notes section for details.

The original SVG files from CyberBrokers are contained in these folders.
- svg-ipfs - These are the SVG files that were placed in IPFS and are referenced in the metadata.  These have svg layer id tags as text descriptors.
- svg-render - These come directly from rendering the NFT via the contract.  These have svg layer id tags as numbers, to save space.

Other than the different in id tag format, both of these are identical version of the NFTs.  The svg-render version may be more useful for those that want to turn on/off layers of a given NFT in an application, as the contract provides id tags in numbers, not text descriptors.

The following additional formats are provided for ease of use.
- svg-nb - The NFTs without their background image.
- svg-card - The NFTs overlayed with a Broker Card, providing metadata information in a single image.

PNG versions of all the above are also provided.  These are rendered at the same resolution as the SVG version.

Not all tools do a good job of converting SVG to PNG, JPG, or any raster format.  I recommend the following tool for linux.  It also has great options for changing the resolution during conversion to take advantage of the SVG file format.
- [rsvg-convert](https://wiki.gnome.org/action/show/Projects/LibRsvg?action=show&redirect=LibRsvg) part of the librsvg package available on most linux varients.

