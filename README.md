# Purpose
This tool downloads the latest raspbian image and sets up g_cdc module to run at bootime to allow for a raspberry pi to be setup with out a monitor or keyboard.

# How to use it
Run the script `sudo ./raspimage`
- raspbian_lite_latest will be downloaded, extracted, and edited.
- When finished, run the command that is output to burn the image to a SD card. 

View options `sudo ./raspimage --help`


# How it works
The script downloads the latest .zip file containing the raspbian image, unzips it, configures g_cdc module to start at boot time (by default) to allow for headless access.

## Additional functions
The script has flags like `-m` for downloading and mounting the image locally in ./boot and ./root respectively to make changes.
