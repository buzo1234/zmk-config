# Piantor Pico 2 keymap

The production firmware is a wired, full-duplex ZMK split. The left half is the only central and the only half intended to connect to the host over USB. The right half is a peripheral.

Four thumb keys are layer-taps: tap for their normal key and hold for the named layer.

```text
Left Alt | GUI | Backspace/Numbers     Space/Symbols | Enter/Mouse | Right Alt/Function
```

## Base

```text
Tab   Q W E R T        Y U I O P Backspace
Ctrl  A S D F G        H J K L ; '
Shift Z X C V B        N M , . / Shift
          Alt GUI Backspace    Space Enter Alt
```

## Numbers

The top row follows the same left-to-right order as a Mac keyboard. Grave is on the far-left home position, and `H/J/K/L` provide left/down/up/right arrows. Other keys are transparent and retain their Base behavior.

```text
1 2 3 4 5 6        7 8 9 0 - =
` · · · · ·        ← ↓ ↑ → · ·
· · · · · ·        · · · · · ·
```

## Symbols

The top row contains the shifted forms of the Number layer in the exact same physical positions. Tilde shares Grave's position. Round, square, and curly brackets are stacked vertically in the same two right-hand columns. Existing Base punctuation stays transparent instead of being duplicated.

```text
! @ # $ % ^        & * ( ) _ +
~ · · · · ·        · · [ ] \ |
· · · · · ·        · · { } · ·
```

## Function

F1-F12, system navigation, media and brightness controls. The right-hand controls are arranged as follows:

```text
H: Brightness up       J: Previous       K: Play/Pause      L: Next
N: Brightness down     M: Mute           ,: Volume down     .: Volume up
```

The left inner thumb sends the macOS Globe/Fn key while the Function layer is active.

The outer bottom keys provide source-local bootloader/reset access for each half.

## Mouse

Hold the right middle Enter thumb to activate the mouse layer. All left-half keys are disabled on this layer; only the right half controls the pointer.

```text
Scroll left | Scroll down | Scroll up | Scroll right | Back | Forward
Mouse left  | Mouse down   | Mouse up  | Mouse right  | Left click | Right click
Left click  | Middle click | Right click | Back | Forward | Disabled
                         Mouse hold | Left click | Right click
```

## Flashing and cable safety

- Flash `piantor_pico2_left.uf2` to the left half.
- Flash `piantor_pico2_right.uf2` to the right half.
- Power the completed keyboard from the left half only.
- Never insert or remove the TRRS cable while either half is powered.
