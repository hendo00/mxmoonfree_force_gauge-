# mxmoonfree_force_gauge-1000N
This repo to help communicate with a mxmoonfree device.
- Device: https://www.amazon.co.uk/Mxmoonfree-Calibration-Certificate-Compression-Destructive/dp/B0DHXWTWLT?source=ps-sl-shoppingads-lpcontext&ref_=fplfs&smid=A2KVF7QXNCLV8H&th=1
- Requirements:
  - Advanced serial port monitor software (windows)
  - Mxmoonfree software (Ask manufacturer)
- Steps:
1. Open Advanced serial port monitor in spy mode.
2. Use the Mxmoonfree software to record some readings.
3. Check the line after the "TX" in Advanced serial port monitor to know the enable string/char.
4. Modify the code attached to "self.board.write(b'e')" and replace the 'e' with your enable character or string.
