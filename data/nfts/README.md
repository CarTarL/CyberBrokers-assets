# CyberBrokers NFT data

This folder contains CSV and JSON formats of all metadata + additional information for all 10,0001 CyberBrokers.

## File Format
- nftId - the token number of the NFT (1)
- name - the broker's name (1)
- talent - one of 51 Talents (1) 
- class - one of 6 Classes (1)
- Species - one of 14 Species (1)
- Gender - female|male|unknown.  derived from layer information
- dna - an integer value that defines all values of the NFT (1)
  - CSV the value is prepended with a tab character to prevent Excel turning this into a number
- mind - integer value 0-30 for Mind statistic (1)
- body - integer value 0-30 for Body statistic (1)
- soul - integer value 0-30 for Soul statistic (1)
- totalStats - mind + body + soul.  integer value 0-90
- layerBkgd - the layer id of the NFT background.  -1 for no background (2)
- minter - the Ethereum wallet address for the original minter of the NFT (2)
- svgAws - a URL to the SVG file for the NFT on Amazon AWS (3)
- svgIpfs - the IPFS link to the SVG file1 (2)
- numTraits - the number of unique traits for the NFT.  integer value 0-12.  This value does not count Talent, Class, or Species
- traits (1)
  - CSV contains columns for trait1 -> trait12.  
  - JSON is array with trait values 
 - layers (2)
   - CSV contains list of layer ids, in order from back to front, that are used in this NFT.  separated by | symbol
   - JSON is array with layer ids, in order from backa to front, that are used in this NFT
 talentDesc - text description of the associated Talent of the NFT (1)

(1) indicates a value directly from the metadata

(2) from contract

(3) from original metadata during mint
