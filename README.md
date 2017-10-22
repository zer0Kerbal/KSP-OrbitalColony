
### Assets
- Taken from [original CivilianPopulation](https://github.com/rabidninjawombat/CivilianPopulation)
- Fixed texture references in every model files
- Some textures were missing just duplicated from existing ones

### Parts
- Structural parts taken from [latest CivilianPopulation](https://github.com/rleroy/CivilianPopulation)

### Configs
- Following parts have internals commented out
	- ApartmentsSmall.cfg
	- ApartmentsLarge.cfg
	- ApartmentsMedium.cfg

### TODO
- convert all textures to dds
- modify mu files to use dds

### MM patches
- Taken from [latest CivilianPopulation](https://github.com/rleroy/CivilianPopulation)

### Convert MM patches from CivilianPopulation
```
#!/bin/bash
sed -i -e 's/t1CivilizationGenerationShipQuartersLarge/OrbitalColonyApartmentsLarge/g' *
sed -i -e 's/t1CivilizationGenerationShipQuartersMedium/OrbitalColonyApartmentsMedium/g' *
sed -i -e 's/InsituKerbalRecruiterTest/OrbitalColonyApartmentsSmall/g' *
sed -i -e 's/surfaceAttachHouseSmall/OrbitalColonyApartmentsTiny/g' *

sed -i -e 's/t1civGardenBiosphere/OrbitalColonyGardenBiosphereLarge/g' *
sed -i -e 's/t1civGardenBiosphereMedium/OrbitalColonyGardenBiosphereMedium/g' *
sed -i -e 's/t1civSmallGardenModule/OrbitalColonySmallGarden/g' *

sed -i -e 's/ndflightSchool/OrbitalColonyAdministrationDeck/g' *
sed -i -e 's/ndMovieTheater/OrbitalColonyMegaBlastTheater/g' *
sed -i -e 's/nduniversity/OrbitalColonyScienceDeck/g' *
```
