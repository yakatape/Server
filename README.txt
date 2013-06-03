CasparCG Server 2.0.3
=====================

Thank you for your interest in CasparCG Server, a professional 
software used to play out and record professional graphics, audio and video 
to multiple outputs. It has been in 24/7 broadcast production since 2006.

This release is considered tested and stable, and is intended for use in
professional production.

More information is available at http://casparcg.com/


SYSTEM REQUIREMENTS
-------------------

1. Intel processor capable of using SSSE3 instructions. Please refer to
   http://en.wikipedia.org/wiki/SSSE3 for a complete list.
   While AMD processors should work, CasparCG Server has only
   been tested on Intel processors.

2. We recommend Windows 7 (64-bit,) but this software has also been used
   successfully on Windows 7 (32-bit) and Windows XP SP2 (32-bit only.) 
   Using CasparCG Server on Windows 8 and Windows Vista is untested and 
   is not recommended!
   
3. An NVIDIA graphics card (GPU) capable of OpenGL 3.0 or higher is required! 
   Please check your card's capabilities at: 
   http://en.wikipedia.org/wiki/Comparison_of_Nvidia_graphics_processing_units

Also make sure that you have the latest drivers installed:
   http://www.nvidia.com/Download/index.aspx?lang=en-us%20nVidia%20drivers
   
   Graphics cards from other manufacturers _may_ work but have not been tested!

4. Microsoft Visual C++ 2010 Redistributable Package must be installed.
   Free download at:
   http://www.microsoft.com/download/en/details.aspx?id=5555

5. You must have Flash Player 10.3 or later installed (an installer can be found
   in the "Flash Player Installation" folder.)

6. Make sure you turn off Windows' "Aero" theme and "ClearType" font smoothing 
   as they have been known to interfere with transparency in Flash templates, 
   and can also cause problems with Vsync when outputting to computer screens.

The latest system recommendations are available at:
http://casparcg.com/wiki/CasparCG_Server#System_Requirements


INSTALLATION
------------

1. Check that your system meets the requirements.

2. Unzip and place the "CasparCG Server 2.0.3" folder anywhere you like.

3. Install "Microsoft Visual C++ 2010 Redistributable Package" from
   http://www.microsoft.com/download/en/details.aspx?id=5555
   
4. Install "Flash Player 10.3.183.14" from the "Flash Player Installation"
   folder.

5. Make sure you turn off Windows' "Aero Theme" and ClearTyper as they can
   interfere with CasparCG Server's OpenGL features!

6. Configure the server settings in the "casparcg.config" text file.

7. Start the "CasparCG.exe" program.

8. Connect to the server from a client, such as the included CasparCG 2.0 Demo
   Client (requires Adobe AIR) or the CasparCG Client 2.0 (available as a
   separate download.)


DOCUMENTATION
-------------

The most up-to-date documentation is always available at
http://casparcg.com/wiki/


CONFIGURATION
-------------

By default, CasparCG Server will look in the media folder for videos, audio and
images files. Flash templates are stored in the templates folder. If you want to
change the location (for example to a faster disk) you just change the paths in
the casparcg.config file.

* How to enable Screen consumer:

  Open casparcg.config and use the following node for consumers:

  <consumers>
      <screen />
  </consumers>

* How to enable a DeckLink card and how to get video in and key output:

  Open casparcg.config and use the following node for consumers:

  <consumers>
      <decklink />
  </consumers>

# Tip:

At the bottom of the casparcg.config file you will find comments which document
additional settings.


LICENSING
---------

CasparCG Client is distributed under the GNU General Public License GPLv3 or
higher, see LICENSE.TXT for details.

The included software is provided as-is by Sveriges Televison AB.
More information is available at http://casparcg.com/
