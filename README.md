Android Image Kitchen for Linux x32, x64.

Credit:
Original author : osm0sis - https://github.com/osm0sis
Ndrancs : make x32 + x64 bit version. - https://github.com/ndrancs -- facebook.com/ndrancs

Tools to build the BIN files:
- Alphat32 Linux OS
- Aboriginal Cross Compiler - September 9, 2014

Device to test new-boot.img generated by this AIK:
- Xperia M Single

Result:
- unpack, repack kernel without problem.
- This compression: gzip, lzma, xz and lzo is work, except lz4,
  because the kernel itself must be lz4 support enable.
- my xperia m use gzip as default

Usage:
On 32bit Linux:
to unpack kernel img
./unpackimg.sh boot.img

to repack
./repackimg.sh

On 64bit Linux:
to unpack kernel img
./unpackimg_x64.sh boot.img

to repack
./repackimg_x64.sh

# android-pack-repack-lin32-lin64
