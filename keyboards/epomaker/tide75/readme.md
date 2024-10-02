# EPOMAKER TIDE 75

---

**WARNING: Do not flash this yet if you care about RGB since the RGB matrices are currently jumbled up, and as a result, per-key effects are all over the place and the CTRL key won't light up.** 

This is most likely the fault of EPOMAKER themselves, as their very own [repo for the tide75](https://github.com/Epomaker/tide75) exhibits the same issue when the VIA or stock QMK firmware contained within is flashed onto the board. I am currently waiting on a response from EPOMAKER themselves and from @sdk66 who seems to be the main firmware developer for this board.

Also, this firmware is currently not on the main QMK repo since EPOMAKER hasn't provided wireless code for the board as off yet, see [this PR](https://github.com/qmk/qmk_firmware/pull/23552#issue-2250038042), and [this one too](https://github.com/qmk/qmk_firmware/pull/23552) for more info.

There is also another slight bug present of the rotary encoder needing to be spun twice to register, once again stemming directly from the firmware provided by EPOMAKER.

---

* Keyboard Maintainer: EPOMAKER(https://github.com/Epomaker)
* Hardware Supported: EPOMAKER TIDE 75
* Hardware Availability: [epomaker](https://www.epomaker.com)

Make example for this keyboard (after setting up your build environment):

    make epomaker/tide_75:default
        
Flashing example for this keyboard:

    make epomaker/tide75:default:flash

To reset the board into bootloader mode, do one of the following:

* Hold the Reset switch mounted on the bottom side of the PCB while connecting the USB cable
* Hold the Escape key while connecting the USB cable (also erases persistent settings)
* Fn+R_Shift+Esc will reset the board to bootloader mode if you have flashed the default QMK keymap

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).
