# lfs-journey
My Linux From Scratch journey


## 17.06.2024

### Reading Progress

Today, I began my Linux From Scratch (LFS) journey using the LFS Book, version 12.1. I covered:

- **Preface:** Provided an overview of the LFS project, explaining its purpose and benefits.
- **Chapter 1: Introduction:** Introduced the project's goals, prerequisites, and tools, emphasizing the educational value of building a Linux system from scratch.

### Additional Reading

I also read two recommended articles:

1. [Software-Building-HOWTO](https://tldp.org/HOWTO/Software-Building-HOWTO.html)
   - Detailed guide on building software from source, including obtaining, configuring, compiling, and installing software.

2. [Beginner's Guide to Installing Software from Source in Linux](https://moi.vonos.net/linux/beginners-installing-from-source/)
   - Beginner-friendly steps for installing software from source, covering dependencies and troubleshooting tips.

### Summary

Today's activities provided a solid foundation for my LFS journey, combining theoretical knowledge from the book with practical insights from the articles.


## 18.06.2024

### Reading Progress

Today I covered:

- **Chapter 2: Preparing the Host System**
  - Set up the necessary tools and environment for the LFS build, including creating and formatting a new partition, setting up the $LFS variable, and mounting the partition.

- **Chapter 3: Packages and Patches**
  - Collected all the required packages and patches needed for the LFS build, ensuring I have everything ready for the installation process.

- **Chapter 4: Final Preparations**
  - Created a basic directory structure, added a dedicated LFS user, set up the build environment, and learned about Standard Build Units (SBUs) and the importance of test suites.

- **Chapter 5: Compiling a Cross-Toolchain**
  - Built the initial cross-compiler tools, including Binutils (Pass 1), GCC (Pass 1), Linux API headers, Glibc, and the C++ standard library (Libstdc++).

### Summary

Today's activities have laid a strong foundation for my LFS build. I've set up my environment, prepared the necessary tools and packages, and completed the first stages of building a cross-compiler.


## 19.06.2024

### Reading Progress

Today, I covered:

- **Chapter 6: Cross Compiling Temporary Tools**
  - Built temporary tools including M4, Ncurses, Bash, Coreutils, Diffutils, File, Findutils, Gawk, Grep, Gzip, Make, Patch, Sed, Tar, Xz, Binutils (Pass 2), and GCC (Pass 2).

- **Chapter 7: Entering Chroot and Building Additional Temporary Tools**
  - Set up the chroot environment by changing ownership, preparing virtual kernel filesystems, entering the chroot environment, creating necessary directories, and setting up essential files and symlinks. Also built additional tools like Gettext, Bison, Perl, Python, Texinfo, and Util-linux. Cleaned up and saved the temporary system.

### Summary

Today's activities completed the setup for the new filesystem environment. I finished creating a suite of temporary tools to use for building the final packages and made backups of essential programs and libraries. I also mounted the virtual filesystems from the host system (e.g., /dev, /dev/pts, /proc, /sys, /run, /dev/shm).


## 20.06.2024

### Reading Progress

Today I covered:

- **Chapter 8: Installing Basic System Software**
  - Built the final versions of all essential packages and rebuilt the compiler and libraries to ensure completeness. This included packages like Glibc, GCC, Binutils, and many more, which are crucial for a functional Linux system.

### Installed Packages

- Man-pages-6.06
- Iana-Etc-20240125
- Glibc-2.39
- Zlib-1.3.1
- Bzip2-1.0.8
- Xz-5.4.6
- Zstd-1.5.5
- File-5.45
- Readline-8.2
- M4-1.4.19
- Bc-6.7.5
- Flex-2.6.4
- Tcl-8.6.13
- Expect-5.45.4
- DejaGNU-1.6.3
- Pkgconf-2.1.1
- Binutils-2.42
- GMP-6.3.0
- MPFR-4.2.1
- MPC-1.3.1
- Attr-2.5.2
- Acl-2.3.2
- Libcap-2.69
- Libxcrypt-4.4.36
- Shadow-4.14.5
- GCC-13.2.0
- Ncurses-6.4-20230520
- Sed-4.9
- Psmisc-23.6
- Gettext-0.22.4
- Bison-3.8.2
- Grep-3.11
- Bash-5.2.21
- Libtool-2.4.7
- GDBM-1.23
- Gperf-3.1
- Expat-2.6.0
- Inetutils-2.5
- Less-643
- Perl-5.38.2
- XML::Parser-2.47
- Intltool-0.51.0
- Autoconf-2.72
- Automake-1.16.5
- OpenSSL-3.2.1
- Kmod-31
- Libelf from Elfutils-0.190
- Libffi-3.4.4
- Python-3.12.2
- Flit-Core-3.9.0
- Wheel-0.42.0
- Setuptools-69.1.0
- Ninja-1.11.1
- Meson-1.3.2
- Coreutils-9.4
- Check-0.15.2
- Diffutils-3.10
- Gawk-5.3.0
- Findutils-4.9.0
- Groff-1.23.0
- GRUB-2.12
- Gzip-1.13
- IPRoute2-6.7.0
- Kbd-2.6.4
- Libpipeline-1.5.7
- Make-4.4.1
- Patch-2.7.6
- Tar-1.35
- Texinfo-7.1
- Vim-9.1.0041
- MarkupSafe-2.1.5
- Jinja2-3.1.3
- Udev from Systemd-255
- Man-DB-2.12.0
- Procps-ng-4.0.4
- Util-linux-2.39.3
- E2fsprogs-1.47.0
- Sysklogd-1.5.1
- Sysvinit-3.08

### Summary

Today's activities were focused on building the core components of my Linux system. I completed the installation of essential packages, ensuring the system is properly set up and configured. This stage is crucial as it lays the foundation for a fully functional Linux system.


## My Linux From Scratch Journey - 21.06.2024

### Reading Progress

Today, I covered:

- **Chapter 9: System Configuration**
  - **Introduction:** Overview of system configuration steps.
  - **LFS-Bootscripts-20230728:** Installed and configured the LFS bootscripts.
  - **Overview of Device and Module Handling:** Learned how to manage devices and modules in the system.
  - **Managing Devices:** Set up device management with `udev`.
  - **General Network Configuration:** Configured basic network settings.
  - **System V Bootscript Usage and Configuration:** Learned to manage and configure System V boot scripts.
  - **Configuring the System Locale:** Set up the system locale settings.
  - **Creating the /etc/inputrc File:** Created and configured the inputrc file for readline.
  - **Creating the /etc/shells File:** Created and configured the shells file listing valid login shells.

### Additional Reading

- **udev Daemon:** Learned about the `udev` daemon from [Greg Kroah-Hartman's paper](http://www.kroah.com/linux/talks/ols_2003_udev_paper/Reprint-Kroah-Hartman-OLS2003.pdf).
- **sysfs Filesystem:** Gained insights into the `sysfs` filesystem from [Patrick Mochel's paper](https://mirrors.edge.kernel.org/pub/linux/kernel/people/mochel/doc/papers/ols-2005/mochel.pdf).

### Summary

Today's activities focused on configuring my Linux system. I installed and configured essential bootscripts, managed devices and modules, set up network configurations, and adjusted system locales. Additionally, I deepened my understanding of `udev` and the `sysfs` filesystem, which are crucial for device management.


## My Linux From Scratch Journey - 25.06.2024

### Reading Progress

Today, I completed the final chapters of my LFS Book. I covered:

- **Chapter 10: Making the LFS System Bootable**
  - **Introduction:** Overview of the boot process.
  - **Creating the /etc/fstab File:** Configured the file system table.
  - **Linux-6.7.4:** Compiled the Linux kernel version 6.7.4.
  - **Using GRUB to Set Up the Boot Process:** Installed and configured GRUB as the bootloader.

- **Chapter 11: The End**
  - **The End:** Concluded the LFS build process.
  - **Get Counted:** Information on registering my LFS build.
  - **Rebooting the System:** Instructions for the first boot into the new LFS system.
  - **Additional Resources:** Provided further reading and resources.
  - **Getting Started After LFS:** Guidance on what to do next after completing LFS.

### Additional Learning

- **Kernel Configuration:** Learned about the kernel configuration process from [Kernel Configuration in a Nutshell](https://anduin.linuxfromscratch.org/LFS/kernel-nutshell/).

### Summary

Today's activities marked the completion of my LFS build. I compiled the Linux kernel, set up GRUB, and prepared the system for its first boot. Additionally, I learned about kernel configuration, which is essential for customizing and optimizing the kernel for my system.


## My Beyond Linux From Scratch Journey - 26.06.2024

### Reading Progress

Today, I began exploring the Beyond Linux From Scratch (BLFS) book. I covered the following sections:

- **I. Introduction**
  - **Welcome to BLFS:**
    - Learned about the structure and sections of the book, conventions used, and where to get source packages.
    - Reviewed the change log, mailing lists, editor notes, and FAQ for additional support.
  - **Important Information:**
    - Explored notes on building software, the /usr vs /usr/local debate, optional patches, BLFS boot scripts, and handling Libtool Archive (.la) files.
    - Understood the differences between static and shared libraries, locale-related issues, and considerations for going beyond BLFS.

- **II. Post LFS Configuration and Extra Software**
  - **After LFS Configuration Issues:**
    - Covered various topics including creating custom boot devices, console fonts, firmware, devices, and configuring user additions.
    - Learned about system users and groups, Bash shell startup files, and customization of logon messages with /etc/issue.
    - Reviewed random number generation and the /etc/vimrc and ~/.vimrc files for Vim editor customization.

### Activities

- **User Profiles and Terminal Customization:**
  - Created default profiles for my users and personalized the terminal interface for a better user experience.

- **Wireless Configuration:**
  - Attempted to configure my wireless interface and connect to a network but was unsuccessful.
  
- **Installed NetworkManager:**
  - Installed NetworkManager and its dependencies to manage network connections more easily.

### Summary

Today's activities involved familiarizing myself with the BLFS book and beginning the post-LFS configuration. Although I encountered challenges with wireless configuration, I installed NetworkManager to assist with managing network connections. Additionally, I created user profiles and customized the terminal interface to enhance usability.
