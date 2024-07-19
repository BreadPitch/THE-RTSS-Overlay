# THE-RTSS-Overlay
Provides a sleek, yet pretty complete overlay for use with RTSS / RivaTuner Statistics Server.
Made for AMD Ryzen + RDNA 1/2/3, but trimmed down for compatibility with most CPUs and GPUs.

![RTSS Overlay Screenshot OW2 Full](https://github.com/BreadPitch/THE-RTSS-Overlay/assets/55409475/9f643e49-674d-46c8-ab2b-460aee7064d2)

<h1>Features</h1>
<ul>
  <li>Auto-detection of CPU & GPU, auto-selection of vendor logo</li>
  <li>Auto-layout for 8 / 16 core processors</li>
  <li>Dynamic colors based on temperature / utilization / fan rpm, to visualize peaks</li>
  <li>Barchart visualization for real-time metrics, with metric history graph overlay for each barchart</li>
  <li>Visually grouped into these sections:</li>
  <ul>
    <li>FPS, Framerate & Frametime section</li>
    <li>GPU section with Clocks, Temp, Fan, GPU util, VRAM util, GPU PPT/TDC/SoC TDC</li>
    <li>CPU section with Clocks, Temp, Fan, CPU util, DRAM util, CPU PPT/TDC/EDC, clock & util per core</li>
    <li>Water cooling section that shows / hides dynamically, based on availablilty of respective sensors</li>
    <li>Network & WHEA section to check connection & eventual hardware errors</li>
  </ul>
  <li>10 versions, 5 each for <b>font size 100% or 80%</b>. 100% for best readability, 80% to "minimize to the max".</li>
  <ul>
    <li><b>Full version (vertical) with HWiNFO sensors for AMD Ryzen CPU & RDNA 1/2/3 GPU</b></li>
    <li><b>Reduced version (vertical) for AMD RDNA 1/2/3 GPU (HWiNFO)</b> with any CPU (RTSS HAL)</li>
    <li><b>Reduced version (vertical) for Ryzen CPU (HWiNFO)</b>, with any GPU (RTSS HAL)</li>
    <li><b>Reduced version (vertical) for all CPS + GPUs (RTSS HAL)</b> with maximum compatibility</li>
    <li><b>Horizontal version (RTSS HAL)</b> for compatibility with games that look best with top bar overlays</li>
  </ul>
</ul>

<h1>Installation Instructions</h1>
<ul>
  <li>Dowload & install RTSS from https://www.guru3d.com/download/rtss-rivatuner-statistics-server-download/</li>
  <ul>
    <li>Activate <b><i>Use Microsoft Detours API hooking</i></b> under <b><i>SetUp / General / Injection properties</i></b> for compatibility</li>
    <li>Activate <b><i>Enable benchmark mode</i></b> under <b><i>SetUp / General / Compatibility properties</i></b></li>
  </ul>
  <li>Download the .zip file from this site and copy all files into <b><i>C:\Program Files (x86)\RivaTuner Statistics Server\Plugins\Client\Overlays</i></b></li>
  <ul>
    <li>Doubleclick <b><i>Lato-Regular.ttf</i></b> and install the Lato Regular font</li>
    <li>Make sure the font is set in the RTSS Main Settings under <b><i>On-Screen Display rendering mode / Raster 3D</i></b> (Lato / Regular / 7)</li>
  </ul>
    <li>Download & install HWinfo from https://www.hwinfo.com/download/</li>
  <ul>
    <li>I prefer portable version, just copy <b><i>HWiNFO64.EXE</i></b> to <b><i>C:\Program Files (x86)\RivaTuner Statistics Server\Plugins\Client\Overlays</i></b>. This way it will use the HWiNFO64.INI file that I provide in the package with my recommended settings.</li>
    <li>Start HWiNFO from there and activate <b><i>Shared Memory Support</i></b> in HWinfo settings under <b><i>Settings / Main Settings</i></b>. Needs to be re-enabled every 24 hours, or you need to buy the Pro version.</li>
  </ul>
</ul>
In RTSS finally
<ul>
  <li>Enable the RTSS OverlayEditor in RTSS under <b><i>Setup / Plugins / OverlayEditor.dll / Layouts / Load</i></b></li>
  <li>Load your preferred .ovl file you just unpacked to <b><i>C:\Program Files (x86)\RivaTuner Statistics Server\Plugins\Client\Overlays</i></b></li>
  <li>I recommend setting also Hotkeys to switch on/off the Overlay and start/stop benchmark recording. Go to <b><i>Setup / Plugins / HotkeyHandler.dll</i></b>. I use CTRL+M to Show OSD, CTRL+N to Hide OSD, CTRL+. to Start Recording, CTRL+, to end recording.
</ul>

<b>Second screen: if you want to use the Overlay on a 2nd screen</b>
<ul>
  <li>Start <b><i>C:\Program Files (x86)\RivaTuner Statistics Server\DesktopOverlayHost.exe</i></b></li>
  <li>Configure an RTSS application profile for <b><i>DesktopOverlayHost.exe</i></b> with the Overlay window position in the upper left corner, and adjust the window to the overlay size. In "Global" profile turn "On Screen Display support" = OFF, or deactivate the OSD for each individual game using application profiles in the RTSS settings.</li>
</ul>

<b>See Screenshots for all relevant settings in the "Additional supportive screenshots" section below.</b>

<h1>Screenshots</h1>

The standard version is ideal for Ultra-Wide Displays, like UWQHD / 3440x1440p, this is what it looks like in OW2:

![RTSS Overlay Screenshot OW2](https://github.com/BreadPitch/THE-RTSS-Overlay/assets/55409475/7e3958df-6feb-4f85-813d-9ee6a1deefd2)

This is what it looks like in 3DMark Timespy running in standard 2560x1440p on a 3440x1440p screen, where it works like a 2nd screen:

![RTSS Overlay Screenshot 3DMark](https://github.com/BreadPitch/THE-RTSS-Overlay/assets/55409475/38f0d4b6-f779-4167-9214-e15d9d24c89c)

It also offers reduced versions, one for RDNA GPUs + Intel / all CPUs, and a compact version based on RTSS HAL only for maximum compatibility with all hardware & games:

![RTSS Overlay Screenshot 3DMark reduced](https://github.com/BreadPitch/THE-RTSS-Overlay/assets/55409475/4141732f-0618-457a-9ac6-cce020ec6a96)

Finally the compact version in horizontal layout:

![RTSS Overlay Screenshot 3DMark horizontal](https://github.com/BreadPitch/THE-RTSS-Overlay/assets/55409475/a64c6bd2-2d1f-4bc8-97fb-af9ce1950fa3)

<h1>Support</h1>

For RTSS Overlay Editor tips to customize the overlay to your CPU, GPU and/or mainboard, please refer to: https://forums.guru3d.com/threads/rtss-overlay-editor-megathread.436443/

The only tip specific to my overlay:
<ul>
  <li>50% transparency is the default pre-set
    <ul>
      <li>For me is the ideal balance of blending into the game, and contrast to see all the nice telemetry.</li>
      <li>You can tune transparency though by simply replacing the color codes in the .ovl file. Simply open it in eg. notepad++ and for all fixed color text elements in white, replace all instances of "=<b>80</b>FFFFFF" (50% transparency) by eg "=<b>CC</b>FFFFFF" for 80% transparency, or "=<b>99</b>FFFFFF" for 60% transparency.</li>
      <li>Same can be done for replacing the dynmic colors, here, I would edit the entire dynamic color line and replace it per element, eg. the temperature values in the detailed tables. Though I suggest to keep the bars in 50% transparency, as this is what makes it possible to display the barchart history with 100% transparency on top of it.</li>
    </ul>
</ul>

<h1>Additional supportive screenshots</h1>

RTSS Font, Compatibility & Layout Settings:

![RTSS Settings 1](https://github.com/BreadPitch/THE-RTSS-Overlay/assets/55409475/d2ec97f2-e551-4f54-9573-53d026fe892e)

RTSS OSD Position, Hotkeys & HWiNFO settings:

![RTSS Settings 2](https://github.com/BreadPitch/THE-RTSS-Overlay/assets/55409475/cff75296-2a22-4f28-87e9-6bbec18ec5ac)

2nd screen configuration:

![2nd screen setup](https://github.com/user-attachments/assets/f25272ee-6021-4198-8f10-9c00de0a7e47)
