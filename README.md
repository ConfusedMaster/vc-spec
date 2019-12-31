# Vietcong data-files specification

This project aims to document as many file formats used by Vietcong game as possible.
We use mainly Python scripts and
[Veles](https://github.com/codilime/veles)
for documenting each file format (there is no official specification and also no disassembling is used during this process).

Python scripts are stored in *scripts* directory.
There is mostly one script per file format.
They are used for verifying that our specification (stored in *doc* dir) is compatible with files distributed by Vietcong game or generated by official utils (such as game editor or 3DS Max plugins).
Sometimes they have more functionality, type -h for help.

We also
[forked](https://github.com/OpenVietcong/veles)
Veles binary analysis tool for better understanding of each file format (it helps us understand meaning of each byte of file by aplying certain parsers).

Specification of CBF file format is partly based on
[vietcong-unpacker](https://github.com/Romop5/vietcong-unpacker)
project.

# File formats with full specification
* [CTR](https://github.com/OpenVietcong/vc-spec/blob/master/doc/ctr.md)
  (Control) - control files.
* [WAY](https://github.com/OpenVietcong/vc-spec/blob/master/doc/way.md)
  (Waypoints) - vehicle waypoints.

# Known file formats

* [BES](https://github.com/OpenVietcong/vc-spec/blob/master/doc/bes.md)
 (BenyErikSolitude) - 3D model.
Contains references to other sources, like textures.
Documented around 90% of version *100*.
Known tools:
  * [3DS MAX 5.1/6/7/8 plugins](http://www.vietcong.info/portal/downloads.php?cat\_id=2)
  * [Blender plugin](https://github.com/sonicpp/vietcong-blender-plugins)
* [CBF](https://github.com/OpenVietcong/vc-spec/blob/master/doc/cbf.md)
(CompressedBigFile) - archive containing encrypted/compressed files.
Documented around 95% for both *ZBL0* and *ZBL1* versions.
Known tools:
  * [Total Commander plugin](http://www.vietcong-coop.net/site?node_id=6&action=show_data&p_id=510&ordercol=fileclass&ordertype=ASC&row=41)
* EQP (Equipment)
* FNT (Font)
* [MANM](https://github.com/OpenVietcong/vc-spec/blob/master/doc/manm.md)
 (ModelAnimation) - describes animation of certain model from BES file.
Documented around 40%.
* [SCO](https://github.com/OpenVietcong/vc-spec/blob/master/doc/sco.md)
 (SceneObject) - level scene.
Contains position of game objects, like models, waypoints etc.
Documented around 1%.
Known tools:
  * [Vietcong Editor](http://www.vietcong.info/portal/downloads.php?cat\_id=2)
  * [Vietcong dev editor](http://www.vietcong.info/portal/downloads.php?cat\_id=2)
* SCR (Script) - compiled from Script ANSI C source code

# Unknown file formats

* LCP
* LDT
* OCT
* PTL
* SCC
* SHM
* SSC (sound?)
* STD
* STG
* STO (skelet animation?)
* TX3
* XDT
* XST
* XTL

# Generic file formats

Images:
* [BMP](https://en.wikipedia.org/wiki/BMP_file_format)
* [DDS](https://en.wikipedia.org/wiki/DirectDraw_Surface)
* [JPG](https://en.wikipedia.org/wiki/JPEG)
* [TGA](https://en.wikipedia.org/wiki/Truevision_TGA)

Audio:
* [OGG](https://en.wikipedia.org/wiki/Ogg)
* [WAV](https://en.wikipedia.org/wiki/WAV)

