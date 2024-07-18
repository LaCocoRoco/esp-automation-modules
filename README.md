## Module Modes

Modes can be changed by pressing de Mode Button. <br />
An audio signal will give feedback of the active mode. <br />
Holding the Mode Button for more then two seconds will clear the module.

### Low Power Mode

- Feedback with one audio signal
- All web functionality is disabled
- Device will go into deep sleep when inactive
- Battery lifetime of serveral month

### Hyprid Mode

- Feedback with two audio signals
- All web functionality is disabled
- Device will go into deep sleep when battery voltage below 3.8V
- Battery lifetime of serveral days

### Web Mode

- Feedback with three audio signals
- All web functionality is enabled
- Battery lifetime of serveral hours

## $\color{red}{\textsf{Importend}}$

All modules have three different modes: Web Mode, Hybrid Mode and Low Power Mode.<br />
The Wi-Fi can be configured as either Access Point or Station Mode.<br />
However, due to the use of the EspNow protocol for communication, there are some restrictions.

### Modules all setup as Access Point (Default):

- All modes work without any restrictions.

### Modules all setup in Station Mode:

- Web Mode works without any restrictions.
- Low Power Mode and Hybrid Mode only work if the Wi-Fi network is set to a **fixed channel**.

### Modules setup in Access Point or Station Mode:

- All modes only work if the Wi-Fi network is set to **channel 1**.

### Explanation

The main goal of this project was to avoid reliance on any infrastructure. For configuration, neither an application nor an existing Wi-Fi network is necessary. All modules can be accessed via the corresponding SSID in Access Point Mode or via hostname in Station Mode. However, there are some trade-offs:

To reduce power consumption in Low Power Mode, the module does not establish a direct network connection. It only broadcasts data to the specified receiver. In Station Mode, the network may change the Wi-Fi channel occasionally. Connecting to the network to receive this information would significantly increase uptime.

An alternative approach to this problem would be to scan for the receiver and request the channel. However, this has additional drawbacks:

- Scanning for this information takes some time (though less compared to connecting to a Wi-Fi network).
- It is difficult to distinguish whether a transmission failure is due to the wrong channel or a general network issue.
- Continuously requesting this information until a response is received would quickly add to the uptime and increase power consumption.

#### Information regards this codebase

Due to the lengthy development process and numerous necessary workarounds, the final codebase feels like a patchwork. Ideally, it should be rewritten from scratch. However, this would require extensive time for redevelopment and retesting. Since there is no significant benefit to doing so, the code will continue to be used in its current form.

##### For future Reference

## Reference

- [VSCode](https://code.visualstudio.com/) - Lighthweight Code editor.
- [PlatformIO](https://platformio.org/) - Embedded Software Development Gateway.
- [Autodesk Fusion 360](https://www.autodesk.com/products/fusion-360) - Design and manufacturing software for CAD, CAM, CAE, and PCB.
- [Autodesk Eagle](https://www.autodesk.com/products/eagle) - Electronic design automation software for printed circuit boards.
- [JLCPCB](https://jlcpcb.com/) - Reasonably priced PCB Manufacturer.
- [LCSC](https://www.lcsc.com/) - Supplier for a wide selection of electronic components.
- [InteractiveHtmlBom](https://github.com/openscopeproject/InteractiveHtmlBom) - Bill of Materials listing with the ability to visually search for components and their placements.

## Preview

### Control Unit

![function_graphic](https://github.com/LaCocoRoco/esp-module-cu/blob/main/images/esp-module-cu-pcb.png)

### Operating Unit

![function_graphic](https://github.com/LaCocoRoco/esp-module-ou/blob/main/images/esp-module-ou-pcb.png)

### Sensor Unit

![function_graphic](https://github.com/LaCocoRoco/esp-module-su/blob/main/images/esp-module-su-pcb.png)
