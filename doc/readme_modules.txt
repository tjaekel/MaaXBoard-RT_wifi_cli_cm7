Supported Wi-Fi/BT/BLE modules
==============================
  - AzureWave AW-NM191MA
  - AzureWave AW-AM510MA
  - AzureWave AW-CM358MA
  - Embedded Artists 2DS M.2 Module (EAR00386)
  - Embedded Artists 1ZM M.2 Module (EAR00364)
  - Embedded Artists 1XK M.2 Module (EAR00385)


Murata Solution Board settings
==============================
Embedded Artists M.2 module resource page: https://www.embeddedartists.com/m2
Embedded Artists 2DS module datasheet: https://www.embeddedartists.com/doc/ds/2DS_M2_Datasheet.pdf
Embedded Artists 1XK module datasheet: https://www.embeddedartists.com/doc/ds/1XK_M2_Datasheet.pdf
Embedded Artists 1ZM module datasheet: https://www.embeddedartists.com/doc/ds/1ZM_M2_Datasheet.pdf


Board settings
==============
M.2 connector:
  - remove R183
  - add 0Ohm resistor at position R404
  
MaaXBoard-RT:
the M.2 connector is not used, instead change to:
#define WIFI_88W8987_BOARD_MURATA_1ZM_USD
in app_config.h
