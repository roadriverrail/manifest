manifest
========

Instruction to build jellybean for cubieboard
1. Download the source code 
  $git clone https://github.com/cubieboard/manifest.git -b jb-cubieboard
  $repo sync

2. Start to build
  $source build/envsetup.sh
  $lunch 4
  $make

3. Generated firmware image
  $tools/pack-cm.sh

4. Flash to cubieboard
  1) Startup Livesuit program(Linux or Windows)
  2) After selecting the firmware, plug in the micro USB while holding the FEL/U-Boot key,
     and keep the key holding about 3 seconds.

Known Issue:
1. EMAC is not supported yet
2. SATA is not tested
3. LINE-OUT is disable




