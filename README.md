# MaaXBoard-RT_wifi_cli_cm7
 MaaXBoard-RT with WIFI demo (connect to AP, provide an AP)

## SDK example for MaaXBoard-RT:
converted from SDK EVK examples:
modify in app_config.h to:

//#define WIFI_IW416_BOARD_MURATA_1XK_M2
#define WIFI_88W8987_BOARD_MURATA_1ZM_USD

## It works:
* you can connect to your AP (WiFi router) via command line
* you can also create an AP (provided by the MaaXBoard), connect to and ping

## Remarks:
The code runs just fine after a power-cycle or the board was reset!
If you flash a new version - you get an initialization error:
the Murata WiFi chip was not reset and cannot be accessed.
Your project should work fine, if you reset the board (or power-cycle).
(unfortunately - not possible to debug, you lose debugger connection).

## UART:
it uses the Debug UART, the MCU-LINK UART, see "help" there and use commands

