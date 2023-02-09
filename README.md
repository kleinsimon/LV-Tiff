# LV Tiff
 A native TIFF reader and writer for LabVIEW.
 
# Installation
Download the .vip file from the latest release under [Releases](https://github.com/kleinsimon/LV-Tiff/releases). Install it using VIPM.
 
# Features
- Raw Data 2xN 
  - 1 / 8 / 16 / 32 / 64 bit signed and unsigned integer
  - Raw floating point in 32 and 64 bit
  - LV-Image
- Compression
  - Deflate (zip)
  - jpeg
- Reading of strided data (not deeply tested)
- TIFF Tags
  - Predefined tags
  - Custom tags
  - transparent data type conversion to LV Variant
  - Type Check for predefined tags
- Multipage
  - independend compression, type and size of pages
  - conversion to / from LV Image (for 24 bit images)
  
# Not supported
- Writing of strided data (not yet, buggy)
- lossless compression other than deflate (packbits, LZW etc.)
- 64 bit pointers (BigTIFF, maybe later) -> Size limited to 4 GB

# Warning
This library is in development and not throughly tested, although many features work and files are recognized by different viewers. BUT tiff is no easy container format and hard to support in all its flavors. If you find errors (you will), post an issue (or even better, a solution).
 
# Dependencies
- OpenG Zip for deflate compression 
- G-Image for jpeg compression
