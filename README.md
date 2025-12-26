# arduino

## Troubleshooting

### Fatal error on upload

When trying to upload my code i had the following error.

```
A fatal error occurred: Unable to verify flash chip connection (Serial data stream stopped: Possible serial noise or corruption.).
```

I changed the upload speed to 115200 in Arduino IDE's Tools menu, the code uploaded and worked and the error did not occur again.

### TFT_eSPI/User_Setup.h settings that I had success with

```
#define ILI9341_DRIVER
#define TFT_WIDTH  240
#define TFT_HEIGHT 320

#define TFT_MISO 12
#define TFT_MOSI 13
#define TFT_SCLK 14
#define TFT_CS   15
#define TFT_DC   27
#define TFT_RST  33

#define TFT_BL   21
#define TFT_BACKLIGHT_ON HIGH

#define SPI_FREQUENCY  27000000
```
