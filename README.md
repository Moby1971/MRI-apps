# MRI apps

Stand-alone applications with a graphical user interface for the reconstruction and analysis of
preclinical MRI data, in particular data acquired with MR Solutions systems.
Gustav Strijkers, Amsterdam UMC, Biomedical Engineering and Physics.

Each app installs with everything it needs: no MATLAB licence and no Python are required.
These are beta versions.

## Downloads

| App | What it does | macOS (Apple silicon) | Windows | Manual |
|---|---|---|---|---|
| **Retrospective** | Reconstruction of self-gated cardiac and respiratory CINE MRI, with automatic LV segmentation | [0.2.0 (250 MB)](https://github.com/Moby1971/MRI-apps/releases/download/retrospective-v0.2.0/Retrospective-0.2.0-macOS-arm64.dmg) | – | [PDF](manuals/retrospective-manual.pdf) |
| **P2ROUD** | Reconstruction of (undersampled) Cartesian, radial, UTE, ZTE and EPI data | [0.2.0 (130 MB)](https://github.com/Moby1971/MRI-apps/releases/download/p2roud-v0.2.0/P2ROUD-0.2.0-macOS-arm64.dmg) | – | [PDF](manuals/p2roud-manual.pdf) |
| **T1mapp** | T₁ mapping: inversion recovery (Look-Locker), saturation recovery and variable flip angle | [0.2.0 (151 MB)](https://github.com/Moby1971/MRI-apps/releases/download/t1mapp-v0.2.0/T1mapp-0.2.0-macOS-arm64.dmg) | – | [PDF](manuals/t1mapp-manual.pdf) |
| **T2mapp** | T₂ and T₂* mapping | [0.2.0 (151 MB)](https://github.com/Moby1971/MRI-apps/releases/download/t2mapp-v0.2.0/T2mapp-0.2.0-macOS-arm64.dmg) | – | [PDF](manuals/t2mapp-manual.pdf) |
| **ADCmapp** | ADC mapping of diffusion-weighted data | [0.2.0 (100 MB)](https://github.com/Moby1971/MRI-apps/releases/download/adcmapp-v0.2.0/ADCmapp-0.2.0-macOS-arm64.dmg) | – | [PDF](manuals/adcmapp-manual.pdf) |
| **DSCmapp** (MATLAB) | Hemodynamic and vascular maps of the brain from dynamic susceptibility contrast (DSC) MRI | – | [2.0.0 (20 MB)](https://github.com/Moby1971/MRI-apps/releases/download/dscmapp-matlab-v2.0.0/DSCmapp-2.0.0-Windows-setup.exe) | [PDF](manuals/dscmapp-manual.pdf) |

DSCmapp is still the MATLAB app (installed with the free MATLAB Runtime), with the MATLAB app's version number; a Python DSCmapp will follow. Windows installers of the other apps will follow. Earlier versions are on the [Releases](https://github.com/Moby1971/MRI-apps/releases) page.

## Installing on macOS

Requirements: a Mac with Apple silicon (M1 or later) and macOS 26 or later.

1. Open the downloaded `.dmg` and drag the app onto the Applications folder.
2. Open it from Applications. The apps are not signed with an Apple Developer ID, so the first
   time macOS refuses a downloaded app ("Apple could not verify ..."). Click **Done**, open
   **System Settings > Privacy & Security**, scroll down to the line saying the app was blocked,
   click **Open Anyway** and confirm. From then on it opens as any other app.

   Or, instead, once in Terminal (with the app's name):

   ```
   xattr -dr com.apple.quarantine /Applications/T1mapp.app
   ```

"Read me first.txt" inside each disk image has the details for that app, such as the optional
BART toolbox.

## Installing on Windows

Windows 10 or 11 (64-bit). Run the downloaded setup program; DSCmapp's installer also installs the
free MATLAB Runtime it needs. Windows may warn that the publisher is unknown: click **More info**
and then **Run anyway**.

## Contact

Gustav Strijkers, Amsterdam UMC, g.j.strijkers@amsterdamumc.nl

The software is provided as is, for research use. It has been tested with mouse data acquired
with an MR Solutions preclinical 7.0T system, but this does not warrant that it meets your
requirements or works without error. If you use the apps in a publication, please cite them as
the manuals describe.
