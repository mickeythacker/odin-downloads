# Third-Party Notices

Project Odin depends on and interoperates with third-party software, services, data,
and operating-system components. Those materials are not relicensed by the Project
Odin proprietary license.

Each third-party component remains governed by its own copyright, license, terms of
service, privacy policy, attribution requirements, and other applicable conditions.

## Components in the 0.1.8 installers

- Python 3.14 runtime and standard library: Python Software Foundation license
  and incorporated-component notices are reproduced in
  `licenses/PYTHON-LICENSE.txt`. Copyright and terms remain with their owners.
- Tcl/Tk 8.6 user-interface runtime: the license notice is reproduced in
  `licenses/TCL-TK-LICENSE.terms`.
- PyInstaller bootloader: built with PyInstaller under its GPL license with
  the official bootloader exception. PyInstaller states that generated bundles
  may carry a separate application license and do not need its license file:
  https://pyinstaller.org/en/stable/license.html

Market-data services such as CoinPaprika and Coinbase Exchange are contacted
over the network; their data and APIs are not relicensed by Project Odin.
Windows and macOS system components remain under their platform owners' terms.
No third-party name implies endorsement or affiliation.

The build process must review changes to included packages and runtime
components before each public release and update this notice accordingly.
See `docs/legal/RELEASE_LEGAL_CHECKLIST.md` for the broader release review.