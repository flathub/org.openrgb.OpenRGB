# OpenRGB

Open source RGB lighting control that doesn't depend on manufacturer software. [openrgb.org](https://openrgb.org)

## Udev rules

To ensure you have device permissions please install the latest UDEV rules.

* Fedora Linux:

  ```
  sudo dnf install openrgb-udev-rules
  ```

* If you need to install the UDEV rules file manually you can also download the [latest compiled udev rules](https://gitlab.com/CalcProgrammer1/OpenRGB/-/jobs/artifacts/master/raw/60-openrgb.rules?job=Linux+amd64+AppImage&inline=false) from GitLab.

  - Copy this `60-openrgb.rules` file to `/usr/lib/udev/rules.d/`
  - Then reload rules with `sudo udevadm control --reload-rules && sudo udevadm trigger`

See: https://gitlab.com/CalcProgrammer1/OpenRGB/-/blob/master/Documentation/UdevRules.md

## OpenRGB Pipeline (Experimental)

You can install latest experimental builds available in `flathub-beta`:

```bash
$ flatpak remote-add --user flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo
$ flatpak install --user flathub-beta org.openrgb.OpenRGB
```

To run:

```
$ flatpak run org.openrgb.OpenRGB//beta
```
