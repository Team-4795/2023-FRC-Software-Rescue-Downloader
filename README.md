# 2023-FRC-Software-Rescue-Downloader

This is a tool to download all of the essential software for
programming an FRC robot in C++ or Java.

The idea is to enable creation of a "rescue" USB drive for use at
events or schools where the Wifi or Cellular internet service is
too slow to rapidly download needed software for a team or student that
needs it.

Prerequisites:

- the bourne shell or bourne again shell (bash)
- wget, the non-interactive web download tool

On linux, try "sudo dnf install wget" or "sudo apt install wget"
On windows, try cygwin or WSL.

Running the downloader:

	sh frc-downloader

It should create a subdirectory "downloads" containing all of the packages.

Hints on creating the rescue USB drive.

Many usb drives still come formatted with the FAT32 filesystem, which
can't handle files larger than 2GB.  Since some of these files will be
bigger, you'll need to use EXFAT or NTFS.  Reformatting your usb drive is
beyond the scope of this readme. Do be careful to reformat the correct
drive, and to not erase your main system drive!


