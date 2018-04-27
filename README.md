[![Build Status](https://travis-ci.org/nroduit/Weasis.svg?branch=master)](https://travis-ci.org/nroduit/Weasis) [![Codacy Badge](https://api.codacy.com/project/badge/Grade/50bdcb5275a84a9186a8e5d9d9d1b81d)](https://www.codacy.com/app/nicolas.roduit/Weasis?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=nroduit/Weasis&amp;utm_campaign=Badge_Grade) The master branch contains Weasis 3.x.x (requires Java 8+) and the old branches are 2.5.x, 2.0.x (Java 6+) and 1.2.x (Java 6+).

Weasis is a free medical DICOM viewer used in healthcare by hospitals, health networks, and patients.

![Weasis](weasis-distributions/resources/images/about.png)

[General information](https://nroduit.github.io)

[Live Demo with different datasets](https://nroduit.github.io/en/demo)

[Download binary releases](http://sourceforge.net/projects/dcm4che/files/Weasis)

[How to build Weasis](https://nroduit.github.io/en/getting-started/building-weasis)

[Issue Tracker](https://dcm4che.atlassian.net/projects/WEA)


### New features in Weasis 3.0 ###
* Replace JAI with OpenCV (increase performance for all the image processing functions)
* Embedded new codecs within OpenCV compiled for Windows 32/64-bit, Linux x86 32/64-bit and Mac OS X 64-bit.    
	* jpeg-baseline, jpeg-extended and jpeg-lossless (IJG 6b)   
	* jpeg-ls (CharLS 2.0)   
	* jpeg2000 codecs (OpegJPEG 2.3)    
	* DICOM raw (RLE, YBR\_FULL, and YBR\_FULL\_422)
* Supports multi-frame and multiple fragments at the same time
* See [JIRA Release Note](http://www.dcm4che.org/jira/secure/ReleaseNote.jspa?projectId=10090&version=12280)

### General Features: ###
* Flexible integration to HIS or PHR (see [weasis-pacs-connector](https://github.com/nroduit/weasis-pacs-connector))
* Web-based distribution (Java Webstart)
* Desktop portable distribution (Windows, Mac OS X, and Linux)
* Embedded DICOM viewer (portable distribution) in CD/DVD or other portable media
* Can be configured with very low memory footprint. Do not require modern hardware.
* [Multi-language support](https://nroduit.github.io/en/getting-started/translating/)
* [Configuration of preferences](https://nroduit.github.io/en/basics/customize/preferences/) on server-side and client-side
* [API for building custom plug-ins](https://nroduit.github.io/en/basics/customize/build-plugins/)
* DICOM Send (storeSCU and STOW RS)
* DICOM Query/Retrieve (C-GET, C-MOVE and WADO)
* Dicomizer module (allow importing standard images and convert them in DICOM)

### Viewer Features: ###
* Display all kinds of DICOM files (including multi-frame, enhanced, MPEG-2, MPEG-4, MIME Encapsulation, SR, PR, KOS, AU, RT and ECG)
* Viewer for common image formats (TIFF, BMP, GIF, JPEG, PNG, RAS, HDR, and PNM)
* Image manipulation (pan, zoom, windowing, presets, rotation, flip, scroll, crosshair, filtering...)
* Layouts for comparing series or studies
* Advanced series synchronization options
* Display Presentation States (GSPS) and Key Object Selection
* Create key images (Key Object Selection object) by selection
* Support of Modality LUTs, VOI LUTs, and Presentation LUTs (even non-linear)
* Support of several screens and full-screen mode
* Multiplanar reconstructions and Maximum Intensity Projection
* Display Structured Reports
* Display cross-lines
* Measurement and annotation tools
* Region statistics of pixels (Min, Max, Mean, StDev)
* SUV measurement
* Save measurements and annotations in DICOM PR or XML file
* Import CD/DVD and local DICOM files
* Export DICOM with several options (DICOMDIR, ZIP, ISO image file with Weasis, TIFF, JPEG, PNG...)
* Magnifier glass
* Native and DICOM printing
* Read DICOM image containing float or double data (Parametric Map)
* ECG Viewer


## Build Weasis ##

Prerequisites: JDK 8 and Maven 3

See the instructions [here](http://www.dcm4che.org/confluence/display/WEA/Building+Weasis+from+source).
