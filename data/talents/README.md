# CyberBrokers Talent data

This folder contains CSV and JSON formats of information on the 51 CyberBrokers Talents.

## File Format
talent - the unique name of the Talent (1)
cid - a unique integer value from 0-51 for the Talent.  ordering reason unknown (2)
class - one of 6 Classes (1)
species - one of 15 Species (1)
rarity - an integer from 1-51 indicating order of rarity within the Talent.  1 is highest rarity (Source).  51 is lowest rarity (Leftover)
qty - total number of NFTs of the Talent
mindMin - the minimum value (0-30) of the Mind value for all NFTs of the Talent
mindMedian - the median value (0-30) of the Mind value for all NFTs of the Talent.  median is more representative of "middle" verses average for the data set
mindMax - the maximum value (0-30) of the Mind value for all NFTs of the Talent
bodyMin, bodyMedian, bodyMax - same as above for the Body statistitic for the Talent
soulMin, soulMedian, soulMax - same as above for the Soul statistitic for the Talent
traitsMin - the minimum value (0-12) of number of Traits for NFTs of the Talent
traitsMedian - the median value (0-12) of number of Traits for NFTs of the Talent
traitsMax - the maximum value (0-12) of number of Traits for NFTs of the Talent
desc - the Lore description for the talent

(1) indicates a value directly from the metadata
(2) from the contract
