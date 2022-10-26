## Udev rules

To ensure you have device permissions please install the latest UDEV rules.

* Fedora Linux:

  ```
  sudo dnf install openrgb-udev-rules
  ```

* If you need to install the UDEV rules file manually you can also download the [latest compiled udev rules](https://gitlab.com/CalcProgrammer1/OpenRGB/-/jobs/artifacts/master/raw/60-openrgb.rules?job=Linux+64+AppImage&inline=false) from Gitlab.

  - Copy this `60-openrgb.rules` file to `/usr/lib/udev/rules.d/`
  - Then reload rules with `sudo udevadm control --reload-rules && sudo udevadm trigger`

See: https://gitlab.com/CalcProgrammer1/OpenRGB#installing-udev-rules-manually.