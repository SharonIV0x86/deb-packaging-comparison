# Debian packaging comparison
Neutralino builder deb comparison.


### Note on Application Identifiers
The Debian packaging targets use two primary application identifiers during package generation: ``applicationName`` and ``applicationId``. The ``applicationName`` is a human-readable name displayed in desktop environments and application menus, while the applicationId serves as the unique package identifier used for package metadata, installation paths, desktop entry filenames, and icon filenames. During packaging, the generated Neutralino executable is automatically detected from the build output directory and packaged together with resources.neu. The detected executable name is stored internally as the resolved binary name and is used when generating launch commands and desktop integration files. Currently, the Debian packaging targets do not use the cli.binaryName configuration field and instead package the executable that is actually produced by the Neutralino build process.
