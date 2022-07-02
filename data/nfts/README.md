# CyberBrokers NFT data

This folder contains CSV and JSON formats of all metadata + additional information for all 10,0001 CyberBrokers.

## File Format
- nftId - the token number of the NFT*
- name - the broker's name*
- talent - one of 51 Talents*
- class - one of 6 Classes*
- Species - one of 14 Species*
- Gender - female|male|unknown.  derived from layer information
- dna - an integer value that defines all values of the NFT*
- mind - integer value 0-30 for Mind statistic*
- body - integer value 0-30 for Body statistic*
- soul - integer value 0-30 for Soul statistic*
- totalStats - mind + body + soul.  integer value 0-90
- layerBkgd - the layer id of the NFT background.  -1 for no background
- minter - the Ethereum wallet address for the original minter of the NFT
- svgAws - a URL to the SVG file for the NFT on Amazon AWS
- svgIpfs - the IPFS link to the SVG file
- numTraits - the number of unique traits for the NFT.  integer value 0-12.  This value does not count Talent, Class, or Species
- traits
-- CSV contains columns for trait1 -> trait12
-- JSON is array with trait values 

* indicates a value directly from the metadata
