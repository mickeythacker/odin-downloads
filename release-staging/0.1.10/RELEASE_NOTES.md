# Project Odin 0.1.10

This release repairs Windows background collection for packaged installations.

The installer now registers the 15-minute market collector and independent health
watchdog against the installed ODIN application instead of a development Python
environment or source repository.

Packaged Health Reports now validate those installed task actions correctly and
give end-user repair guidance instead of source-tree Python/PowerShell commands.

Uninstalling Odin also removes the packaged scheduled tasks cleanly.

The in-app Help & User Guide and Mímisbrunnr / The Well remain included on Windows,
Apple Silicon Mac, and Intel Mac builds.
