# CyberBrokers Layer data

This folder contains CSV and JSON formats of information on the 1460 SVG layers contained in the CyberBrokers (CB) contract that are combined to create each CB NFT

## File Format
- layerNum - the unique number of the layer 0-1459 (2)
- tagText - the descriptive tag id for the layer which contains a lot of information (3)
- traitType - the category of the Trait, which matches the metadata (2)
- traitName - the Trait value within the category, which matches the metadata (2)
- layerType - a manually assigned category for the layer to help categorize them
  - back - a layer this is the back part of a trait layer
  - background - one of the 100 background layers options for the NFTs
  - body - one of the base body layer options for the NFTs
  - face - one of the base face layer options for the NFTs
  - icon - an icon for one of the 51 Talents
  - other - didn't fit well into the above categories
  - trait - matches a Trait value from the metadata (1)
- gender - if the layer has gender asignment from the tagText, used to determine NFT gender value
- tagId - the top level integer tag id for the layer (2)
- tagIds - all integer tag ids from the layer (2)
  
(1) indicates a value directly from the metadata  
(2) from the contract  
(3) from the IPFS and AWS versions of the NFT SVG files
