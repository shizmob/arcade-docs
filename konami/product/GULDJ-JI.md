# `GULDJ-JI`: Beatmania IIDX PENDUAL LCD monitor

* "PENDUAL LCD"
* Monitor manufacturer: Konami Digital Entertainment
* Panel
  * YTE YING TCHAIN ELECTRONIC CO., LTD
  * Model: RLMV42H-OFC4VNWE7 (AU HVN01.1)
  * Input: DC 24V - 4A
* Size: 42"
  * Visible size is 37". The remainder of the display area is covered by the bezel around the screen
  * The input image is re-sized to the 37" visible area using the zoom feature of the firmware in
    the OSD menu
* Weight: 46kg
* Power
  * Voltage: AC100V
  * Consumption: 100W
  * Rated frequency: 50/60Hz
* Native resolution: 1920x1080
* Input: VGA, DVI
* Known "manufacturing numbers" (`_` are redacted parts creating the unique identifier)
  * `LDJUJIM_____` #WEB:https://twitter.com/kururusky/status/1601190433240936449/photo/1`

## Notes and known issues

* The monitor has different OSD menu items depending on the current screen resolution provided,
  e.g. 1080p vs 720p
* The firmware down-scales the image for 720p with rather poor results
  * Flaky refresh rates of 59.970 hz to 59.990 hz if not enforcing fixed/custom timings via GPU
  * Colors are different compared to 1080p (warmer?)
  * Moving white objects have a yellow-ish gradient which might be a symptom of increased ghosting
  * Display latency feels worse than in 1080p mode, likely due to the down-scaling being expensive
* The 1080p mode does not suffer from all the above and is the recommended operating mode for this
  monitor
* The display's firmware is not capable of adapting to other refresh rates than 60.000 hz correctly
* Driving the display with any different refresh rate and the firmware compensates by occasionally
  dropping frames. This can be tested with a (vsync-tester)[https://www.vsynctester.com] that's
  alternating between frames allowing to spot frame drops. For example, driving the display with
  59.000 hz "works", but drops a frame every second. This results in an occasional stuttering when
  displaying scrolling objects due to a skipped frame by the display (and not by the GPU!)