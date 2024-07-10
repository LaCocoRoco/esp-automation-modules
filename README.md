# $\color{red}{\textsf{In Development}}$

## Quick Guide

> git clone --recursive https://github.com/LaCocoRoco/esp-automation-modules.git

## Sidenotes

- **Code optimization:** Due to the long development time, the codebase was consolidated.The effort required for optimization and separation is not proportional to the time needed.

- **Power consumption:** The power consumption of the individual modules could be optimized. It would be possible to use the ULP processor instead of the DeepSleepWakeStub. However, this would require additional tools and complicating the handling. The hardware could also be revised to reduce power consumption, but the benefits are negligible.

- **Communication:** To reduce power consumption, the communication between the Master (Control Unit) and the Slave (Operating Unit & Sensor Unit) is unidirectional.

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
