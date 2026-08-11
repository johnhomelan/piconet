# CHANGELOG.md

## 2.1.0 (2026-08-11)

Fixes:

 - Fix `_wait_ack` to filter incoming ACK frames by the address a transmission was actually sent from, rather than the board's globally configured station — needed for source station/network overrides to work, but also more correct in general

Features:

 - Allow the source station and network of a single `TX`/`transmit()` operation to be overridden without changing the board's configured station (`SET_STATION`/`setEconetStation`)

## 2.0.20 (2023-06-11)

Fixes:

 - Change TIMEOUT_DATA_FRAME_MS to 100ms to reduce retries on Windows

Features:

 - None

## 2.0.19 (2023-06-11)

Fixes:

 - Handle retries when errors occur receiving frames
 - Generate retries when sent data is not acknowledged
 - Resolve misc. timing issues
 - Better use of flag fill to avoid getting data from server before we're actually ready for it

Features:

 - None

## 2.0.15 (2023-05-31)

Fixes:

 - Improve handling of rx abort in data frame
 - Fix build to allow use of latest Pico SDK (reference pico_sdk_import.cmake in sdk)
 
Features:

 - None

## 2.0.14 (2023-05-30)

Fixes:

 - None
 
Features:

 - First public release
 