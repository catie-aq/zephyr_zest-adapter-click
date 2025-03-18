# Zest_Adapter_Click

Zest_Adapter_Click board support for Zephyr OS.

## Usage

A mikroBUS header is exposed by the overlay, allowing [Click Boards](https://www.mikroe.com/click) to be connected to the Zest_Adapter_Click.

:pushpin: This shield defines:

- a mikroBUS connector: `mikrobus_header`,
- a mikroBUS serial bus: `mikrobus_serial`,
- a mikroBUS I2C bus: `mikrobus_i2c`,
- a mikroBUS SPI bus: `mikrobus_spi`.

:triangular_ruler: To use this shield:

- Update your device tree by adding the `ZEST_ADAPTATER_CLICK(port)` macro to the `app.overlay` file.\
  Replace `port` with the number of the Zest_Core port to which the shield is connected, e.g.:

  ```c
  ZEST_ADAPTATER_CLICK(1) /* Zest_Adaptater_Click connected to Zest_Core first port */
  ```

- Activate support for the shield by adding `--shield zest_adaptater_click` to the west command.
