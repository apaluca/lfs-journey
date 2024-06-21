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
- About Debugging Symbols
- Stripping
- Cleaning Up

### Summary

Today's activities were focused on building the core components of my Linux system. I completed the installation of essential packages, ensuring the system is properly set up and configured. This stage is crucial as it lays the foundation for a fully functional Linux system.

