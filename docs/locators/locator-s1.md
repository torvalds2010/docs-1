# Hardware Setup

## Description

The Locator-S1 is a digital hydro acoustic locator device with an internal GPS based time sync module. The Locator-S1 does not require tether integration for top-side communication. It only requires external power 10-18V to be provided from the underwater vehicle. Some Locator-S1 attributes can be configured using an integrated UART interface. This configuration is optional and not required for normal operation. Before deployment in water, the Locator-S1 needs to achieve a GPS lock. The integrated status-LED shows the condition of the GPS lock.

## Benefits

* GPS based sync removes all tether requirements enabling very easy integration with any ROV.

* Extremely small size making it perfect for even the smallest underwater vehicles.

* Highly robust operation in areas with reflections (shallow water, around installations etc.)

## Wiring interface

The tables below shows the pinning of the S1 interface.

| Interface           | Color |
| :------------------ | :-- |
| Positive (10-18V) | Orange  |
| Negative | Orange/White   |
| UART RX | Brown  |
| UART TX | Brown/White   |

## Terminal Interface

The Locator-S1 has a simple UART interface which is used to change the channel of the locator. 

| Settings           | Value |
| :------------------ | :-- |
| Baud rate | 9600  |
| Data parity stop | 8N1   |
| Flow control | None  |

## Dimensions

![s1_dimensions](../img/s1_dimensions.png)