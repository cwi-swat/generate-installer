generate-installer
==================

A shell script that generates auto extractable shell scripts for installing pre-compiled binaries and relocating them to the installation site on Un*x systems.

How to use this script:
 * Compile and install your arbitrarily complex system into a separate set of directories. Typically these would be the --prefix options of your configure scripts.
    - make sure the absolute path names of the prefixes are as long as possible. This length is what limits the eventual depth of the installation directory at the client side ;-) 
 * Run generate-installer.sh with commandline options to point to the prefixes to package, and possibly external dependencies that should not be included but need to be checked at the client site at installation time.
    - redirect the output to a file that will be the auto-extracting installation script
 * Deploy the generated script on your website.
 * Done!
 
We wish you happy deployment using generate installer.