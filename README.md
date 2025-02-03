[Boppo] is a tablet with 10 light up buttons and a speaker but no screen. I have
been working on it for over 4 years.

By mid 2025 this crate will contain the API used to create activities for the
boppo tablet. I am cleaning up the API for public use.

I have developed over 30 activities at this time but I am most excited to see
what activities others will build for the tablet.

## The Specifications

Boppo's 10 light up buttons contain an RGB LED that can be changed to any RGB
value but bright and saturated colors are best represented (e.g. black is just
off and does not look black).

The buttons are quality mechanical keyboard switches (currently Gateron Green
switches but that is still subject to change).

Boppo is powered by an [ESP32-S3] which is a microcontroller that has:

* a dual-core CPU running at 240 Mhz
* 512 kB SRAM
* At least 2 MB PSRAM
* Wifi and Bluetooth communication

Boppo also has an NFC antenna that can read supported NFC tags.

# The API

The current activities and API are programmed in the  [Rust] programming
language. Additional language integration is possible in the future.

Easy to use functions and structs for receiving input and changing the button
colors are provided.

I also developed a custom audio playback library called [awedio] to support
streaming multiple sounds with effects simultaneously on an ESP-32 which is used
in the SDK.

## Share with Others

Made an activity that you think others will like? Let us know and we will
consider including it in the global list shipped to all devices.

## Open

The circuit board schematic will be available to the public. The [awedio] audio
playback library has been open sourced and the SDK will be open sourced in the
future. I plan to open source more of the platform over time.

[boppo]: https://boppo.com
[Rust]: https://rust-lang.org
[awedio]: https://github.com/10buttons/awedio
[ESP32-S3]: https://www.espressif.com/en/products/socs/esp32-s3
