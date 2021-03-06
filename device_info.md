CEM DT-174B device information
==============================

Summary
-------

 * USB stick data-logger for logging
    * temperature
    * relative humidity
    * air pressure.
 * It uses
    * `Silabs F321 ECLOGG 1217+` controller
    * `24LC512` EEPROM.
 * `lsusb` identifies this device as `ID 10c4:ea61 Cygnal Integrated Products, Inc.`
 * Linux automatically loads driver cp210x for this device, but it doesn't work.

Detailed device identification
------------------------------
By `lsusb -v`

        Bus 002 Device 008: ID 10c4:ea61 Cygnal Integrated Products, Inc. 
        Couldn't open device, some information will be missing
        Device Descriptor:
        bLength                18
        bDescriptorType         1
        bcdUSB               1.10
        bDeviceClass            0 (Defined at Interface level)
        bDeviceSubClass         0 
        bDeviceProtocol         0 
        bMaxPacketSize0        64
        idVendor           0x10c4 Cygnal Integrated Products, Inc.
        idProduct          0xea61 
        bcdDevice            1.00
        iManufacturer           1 
        iProduct                2 
        iSerial                 3 
        bNumConfigurations      1
        Configuration Descriptor:
        bLength                 9
        bDescriptorType         2
        wTotalLength           32
        bNumInterfaces          1
        bConfigurationValue     1
        iConfiguration          0 
        bmAttributes         0x80
        (Bus Powered)
        MaxPower               30mA
        Interface Descriptor:
        bLength                 9
        bDescriptorType         4
        bInterfaceNumber        0
        bAlternateSetting       0
        bNumEndpoints           2
        bInterfaceClass       255 Vendor Specific Class
        bInterfaceSubClass      0 
        bInterfaceProtocol      0 
        iInterface              0 
        Endpoint Descriptor:
                bLength                 7
                bDescriptorType         5
                bEndpointAddress     0x02  EP 2 OUT
                bmAttributes            2
                Transfer Type            Bulk
                Synch Type               None
                Usage Type               Data
                wMaxPacketSize     0x0040  1x 64 bytes
                bInterval               0
        Endpoint Descriptor:
                bLength                 7
                bDescriptorType         5
                bEndpointAddress     0x82  EP 2 IN
                bmAttributes            2
                Transfer Type            Bulk
                Synch Type               None
                Usage Type               Data
                wMaxPacketSize     0x0040  1x 64 bytes
                bInterval               0

