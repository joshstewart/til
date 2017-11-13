There are generally four ways to create a disk image on an OS X box:

    Disk Utility - The on-screen prompts will guide you, but it will by default create a .dmg, which is an OS X-specific file format. Disk Utility will also create an ISO (.cdr extension) if you select the "CD/DVD Master" option before creating the image. You can rename the extension (to .iso) after creation if desired.

    Roxio Toast - The de facto third-party standard in creating optical media on Mac OS for over a decade, it will create almost any CD or DVD format you want.

    The hdiutil command-line utility, which will, in fact, create every format that Toast supports, for free, though it is far less pretty. If you want to create an ISO with this tool, use hdiutil makehybrid -iso -joliet -o Image.iso /input_path

    There is a fourth, extremely direct command-line way using dd that sysadmins might know: dd if=/dev/disk1 of=Image.iso

https://superuser.com/questions/85987/mac-os-x-best-way-to-make-an-iso-from-a-cd-or-dvd
