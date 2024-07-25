# THE-RTSS-Overlay
Provides a sleek, yet pretty complete overlay for use with RTSS / RivaTuner Statistics Server.
Made for AMD Ryzen + RDNA 1/2/3, but trimmed down for compatibility with most CPUs and GPUs.

Can be used both as <b>in-game overlay</b>, or on a <b>second screen</b>.

![RTSS Overlay Screenshot Intro](https://github.com/user-attachments/assets/421ff9ef-b420-4214-bb9e-2b9d77181f56)

![RTSS Overlay Screenshot OW2 Full](https://github.com/user-attachments/assets/3d2ee08b-ba1a-4945-8e5a-84aefc4f63e7)

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

Download & install RTSS from https://www.guru3d.com/download/rtss-rivatuner-statistics-server-download/

Download <i>THE-RTSS-Overlay</i> <a href="https://github.com/BreadPitch/THE-RTSS-Overlay/releases">latest release Source code.zip</a> from this site. From v1.3 on, installation now is much easier. Simply <b>make sure RTSS is closed</b>, and <b>copy the content of the .zip file to the RTSS installation folder</b>, for most users this will be <b><i>C:\Program Files (x86)\RivaTuner Statistics Server</i></b>.
<ul>
  <li>With this, all settings as per manual installation instructions are automatically pre-enabled</li>
  <li>By default, the most universal <i>BreadPitCh-Size100-RTSS-Compact4all.ovl</i> with 100% font size is loaded.
    <ul>
      <li>If you use HWiNFO in the background and want all RDNA & Ryzen metrics from it, load <i>BreadPitCh-Size100-HWinfo-Full-RDNA-Ryzen</i>
      <li>If you do not use HWiNFO, or have an nVidia GPU or Intel CPU, I recommend to stick to <b><i>BreadPitCh-Size100-RTSS-Compact4all.ovl</i></b>, or the -horizontal version, based on your preference</li>
      <li>Simply load your preferred .ovl overlay in the Overlay Editor; after copying / unpacking you find all versions at <b><i>C:\Program Files (x86)\RivaTuner Statistics Server\Plugins\Client\Overlays</i></b>)</li>
    </ul>
  <li><b><i>Lato-Regular.tff</i> in the Fonts folder must still be installed manually</b> by doubleclick --> install</li>
  <li><b><i>DesktopOverlayHost.exe</b></i> is enabled by default, you can turn it off by right-clicking and disabling <i>"Start with Windows"</i>, then close. Alternatively, turn <i>On-Screen Display support = OFF</i> in Global profile, to just use <i>DesktopOverlayHost.exe</i> for 2nd screen.</li>
</ul>

Download & install HWinfo from https://www.hwinfo.com/download/
<ul>
    <li>I prefer portable version, just copy <b><i>HWiNFO64.EXE</i></b> to <b><i>C:\Program Files (x86)\RivaTuner Statistics Server\</i></b>. This way it will use the <i>HWiNFO64.INI</i> file that I provide in the package with my recommended settings.</li>
    <li>Start HWiNFO from there and activate <b><i>Shared Memory Support</i></b> in HWinfo settings under <b><i>Settings / Main Settings</i></b>. Needs to be re-enabled every 24 hours, or you need to buy the Pro version.</li>
  </ul>

<h2>Recommended settings for optimal GPU performance & display quality</h2>

Settings for VRR = FreeSync & G-Sync monitors:
<ul>
  <li>G-Sync / FreeSync ON in GPU drivers. If not available, check in your monitor OSD</li>
  <li>V-Sync ON in GPU driver</li>
  <li>Frame Limiter ON and set to 2-7 FPS less than your monitors refresh rate in Hz, so eg. 144 Hz = 137 FPS frame limit</li>
  <ul>
    <li>Frame Limit ideally set in-game (best input latency)</li>
    <li>If not available in-game, set Frame Limit in RTSS (just a little more latency). Setting it in GPU driver performs worst.</li>
  </ul>
</ul>

Settings for non-VRR monitors: see this <a href=https://forums.blurbusters.com/viewtopic.php?t=4916>BlurBusters</a> how-to.

Sources for more information:
<ul>
  <li>For VRR = FreeSync & G-Sync monitors: <a href=https://blurbusters.com/gsync/gsync101-input-lag-tests-and-settings/14/>BlurBusters</a></li>
  <li>For non-VRR monitors: <a href=https://forums.blurbusters.com/viewtopic.php?t=4916>BlurBusters</a>, <a href=https://forums.guru3d.com/threads/is-someone-able-to-explain-how-async-and-back-edge-sync-differ-thanks.447580/#post-6124964>RTSS author Unwinder</a>, <a href=https://forums.guru3d.com/threads/is-someone-able-to-explain-how-async-and-back-edge-sync-differ-thanks.447580/#post-6124849>RTSS forum</a></li>
</ul>

<h2>Alternative: manual RTSS configuration</h2>
Reminder: all settings are pre-set if you extract / copy all files & folders of the .zip file to the RTSS installation folder.
<ul>
  <li>Download & install RTSS from https://www.guru3d.com/download/rtss-rivatuner-statistics-server-download/</li>
  <ul>
    <li>Activate <b><i>Use Microsoft Detours API hooking</i></b> under <b><i>SetUp / General / Injection properties</i></b> for compatibility, eg. with Witcher 3 FG mod, or to have RTSS & Discord Overlay work alongside in OW2.</li>
    <li>Activate <b><i>Enable benchmark mode</i></b> under <b><i>SetUp / General / Compatibility properties</i></b></li>
    <li>Activate <b><i>Enable frame limiter</i></b> = async under <b><i>SetUp / General / Compatibility properties</i></b></li>
  </ul>
  <li>Download the <a href="https://github.com/BreadPitch/THE-RTSS-Overlay/releases">latest release Source code.zip</a> from this site and copy all files in <b><i>Plugins\Client\Overlays</i></b> to <b><i>C:\Program Files (x86)\RivaTuner Statistics Server\Plugins\Client\Overlays</i></b></li>
  <ul>
    <li>Doubleclick <b><i>Lato-Regular.ttf</i></b> in the Fonts folder and install the Lato Regular font</li>
    <li>Make sure the font is set in the RTSS Main Settings under <b><i>On-Screen Display rendering mode / Raster 3D</i></b> (Lato / Regular / 7)</li>
  </ul>
</ul>
In RTSS finally
<ul>
  <li>Enable the RTSS OverlayEditor in RTSS under <b><i>Setup / Plugins / OverlayEditor.dll / Layouts / Load</i></b></li>
  <li>Load your preferred .ovl file you just unpacked (you find it at to <b><i>C:\Program Files (x86)\RivaTuner Statistics Server\Plugins\Client\Overlays</i></b>)</li>
  <li>I recommend setting also Hotkeys to switch on/off the Overlay and start/stop benchmark recording. Go to <b><i>Setup / Plugins / HotkeyHandler.dll</i></b>. I use CTRL+M to toggle OSD (on/off), CTRL+, to Start Recording, CTRL+. to end recording, and CTRL+- to toggle Frame Limiter (on/off).
</ul>

Finally download & install HWinfo as described above, and copy the HWiNFO64.INI to RTSS installation folder, for most users this will be <b><i>C:\Program Files (x86)\RivaTuner Statistics Server</i></b>.

<h2>Alternative: manual RTSS configuration for second screen - additional steps</h2>
If you want to use the Overlay on a 2nd screen, follow these additional steps:
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

<h2>RTSS Font, Compatibility & Layout Settings</h2>

![RTSS Settings 1](https://github.com/user-attachments/assets/bab1af1c-d0f7-48b1-a2df-7a57f9f246f7)

<h2>RTSS OSD Position, Hotkeys & HWiNFO settings</h2>

![RTSS Settings 2](https://github.com/user-attachments/assets/794a01b6-b60e-4285-b2e4-327c13559462)

<h2>2nd screen configuration</h2>

![2nd screen setup](https://github.com/user-attachments/assets/950e5c14-4937-43bf-9e81-ed32130b55bb)



