Welcome to the oresat-structure wiki!

## Downloading the Repository

1. Clone the repository to your system<be>

`git clone https://github.com/oresat/oresat-structure.git`

> **NOTE:** The repository is around 9GB in size. If you would not like to download the entire repository history, use the following command instead<be>
> 
> `git clone --depth 1 https://github.com/oresat/oresat-structure.git`
> * The --depth 1 flag indicates that only the most recent commit will be cloned
> 
> To also clone all branches, use the following command<be>
> 
> `git clone --depth 1 --no-single-branch https://github.com/oresat/oresat-structure.git`
> * the --no-single-branch flag indicates that all branches should be cloned (since --depth automatically runs --single-branch)

2. Download Solidworks

3. Open up the files to get started!

## Repo Structure
- OreSat.SLDASM  
_The complete assembly of OreSat_
- AssemblyJig
_What we use to hold OreSat on tables/for display_
- Backplane  
_The hub which provides power and data to all the boards_
- BatteryCard 
_The assembly that holds the batteries to the card; includes inhibit switches_
- Cameras
_Parts/subassemblies for the cameras_
- COTS  
_Any Commercial-Off-The-Shelf parts -- screws, connectors, et cetera._
- DebugConnector  
_The connector that allows for easy debugging of the satellite_
- Endcap  
_The boards that are placed on the +Z and -Z ends of the satellite_
- Endcards  
_The cards placed next to the Endcaps; hold the deployable antennas_
- Frames
_The +X and -X Frames, as well as the Y frames; wedges and triangles_
- GenericCard  
_Parts/subassemblies for the generic card; other cards for OreSat_
- LICENSE 
_CERN OHL licensing_
- ReactionWheels
_The wheels that are located in the center of OreSat and help it spin while in orbit_
- Solar  
_Solar panel boards
- VibrationJig  
_The fixtures that hold OreSat on the vibration table during testing_
- VolumeKeepout  
_Solids for quickly checking if we conform to the CDS, by checking for interferences_


## Terminology
These are just some terms that are relevant to the structure, non-obvious to an MME, or non-standard.  
- The X and Z axes are aligned to the features described below, and the Y axis is oriented to obey the right hand rule. The axes of the top-level assembly follow this convention. This convention matches that of our launch provider.
- A _board_ is any printed circuit board (PCB).
- A _card_ a board that slides into the rack structure of the satellite.
- An _endcap_ is a board that is screwed onto one of the +/-Z faces.
- An _endcard_ is a card that slides in under the +Z EndCap or above the -Z EndCap.
- _Rack_ and _structure_ both refer to the assembly of aluminum _frames_ to which all the boards mount.
- The _sides_ are the +/-Y components of the rack. They have the slots that the cards slide into.
- The _-X side_ is the location of the backplane, while the _+X side_ is placed on last, acting somewhat like a lid
- The _backplane_ is the long board that sits on the -X face of the satellite. It transfers power, data, and RF between the boards.
- The _turnstile_ antenna is the four-pronged antenna on the -Z face of the satellite. It provides an omnidirectional, low-data-rate signal to the ground.
- The _helical_ or _high gain_ antenna is the spiral, single-pronged antenna on the +Z face of the satellite. It's the narrow-beam, high-data-rate antenna the satellite uses for transmitting video.