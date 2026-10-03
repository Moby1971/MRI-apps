# MRI apps

<p align="center"><img src="https://moby1971.github.io/MRI-apps/images/banner.png" alt="Retrospective, P2ROUD, T1mapp, T2mapp, ADCmapp and DSCmapp" width="100%"></p>

Stand-alone applications with a graphical user interface for the reconstruction and analysis of
preclinical MRI data, in particular data acquired with MR Solutions systems.
Gustav Strijkers, Amsterdam UMC, Biomedical Engineering and Physics.

Each app installs with everything it needs: nothing else has to be installed.
These are beta versions.

## Downloads

| App | What it does | macOS (Apple silicon) | Manual |
|---|---|---|---|
| <img src="https://moby1971.github.io/MRI-apps/images/icons/retrospective.png" width="32" height="32" align="middle" alt=""> **Retrospective** | Reconstruction of self-gated cardiac and respiratory CINE MRI, with automatic LV segmentation | [0.2.2 (251 MB)](https://github.com/Moby1971/MRI-apps/releases/download/retrospective-v0.2.2/Retrospective-0.2.2-macOS-arm64.dmg) | [PDF](https://moby1971.github.io/MRI-apps/manuals/retrospective-manual.pdf) |
| <img src="https://moby1971.github.io/MRI-apps/images/icons/p2roud.png" width="32" height="32" align="middle" alt=""> **P2ROUD** | Reconstruction of (undersampled) Cartesian, radial, UTE, ZTE and EPI data | [0.2.1 (130 MB)](https://github.com/Moby1971/MRI-apps/releases/download/p2roud-v0.2.1/P2ROUD-0.2.1-macOS-arm64.dmg) | [PDF](https://moby1971.github.io/MRI-apps/manuals/p2roud-manual.pdf) |
| <img src="https://moby1971.github.io/MRI-apps/images/icons/t1mapp.png" width="32" height="32" align="middle" alt=""> **T1mapp** | T₁ mapping: inversion recovery (Look-Locker), saturation recovery and variable flip angle | [0.2.1 (151 MB)](https://github.com/Moby1971/MRI-apps/releases/download/t1mapp-v0.2.1/T1mapp-0.2.1-macOS-arm64.dmg) | [PDF](https://moby1971.github.io/MRI-apps/manuals/t1mapp-manual.pdf) |
| <img src="https://moby1971.github.io/MRI-apps/images/icons/t2mapp.png" width="32" height="32" align="middle" alt=""> **T2mapp** | T₂ and T₂* mapping | [0.2.1 (152 MB)](https://github.com/Moby1971/MRI-apps/releases/download/t2mapp-v0.2.1/T2mapp-0.2.1-macOS-arm64.dmg) | [PDF](https://moby1971.github.io/MRI-apps/manuals/t2mapp-manual.pdf) |
| <img src="https://moby1971.github.io/MRI-apps/images/icons/adcmapp.png" width="32" height="32" align="middle" alt=""> **ADCmapp** | ADC mapping of diffusion-weighted data | [0.2.1 (100 MB)](https://github.com/Moby1971/MRI-apps/releases/download/adcmapp-v0.2.1/ADCmapp-0.2.1-macOS-arm64.dmg) | [PDF](https://moby1971.github.io/MRI-apps/manuals/adcmapp-manual.pdf) |
| <img src="https://moby1971.github.io/MRI-apps/images/icons/dscmapp.png" width="32" height="32" align="middle" alt=""> **DSCmapp** | Hemodynamic and vascular maps of the brain from dynamic susceptibility contrast (DSC) MRI | [0.1.0 (101 MB)](https://github.com/Moby1971/MRI-apps/releases/download/dscmapp-v0.1.0/DSCmapp-0.1.0-macOS-arm64.dmg) | [PDF](https://moby1971.github.io/MRI-apps/manuals/dscmapp-manual.pdf) |

Windows installers will follow.

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

## Contact

Gustav Strijkers, Amsterdam UMC, g.j.strijkers@amsterdamumc.nl

The software is provided as is, for research use. It has been tested with mouse data acquired
with an MR Solutions preclinical 7.0T system, but this does not warrant that it meets your
requirements or works without error. If you use the apps in a publication, please cite them as
the manuals describe.
