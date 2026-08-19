# Piantor Pico 2 keymap

The production firmware is a wired, full-duplex ZMK split. The left half is the only central and the only half intended to connect to the host over USB. The right half is a peripheral.

The four middle thumb keys are layer-taps: tap for their normal key and hold for the named layer.

```text
Left Alt/Function | Backspace/Nav | Space/Numbers     Space/Mouse | Enter/Symbols | Right Alt
```

## Base

```text
Tab   Q W E R T        Y U I O P Backspace
Shift A S D F G        H J K L ; '
Ctrl  Z X C V B        N M , . / Shift
          Alt Backspace Space    Space Enter Alt
```

## Navigation

Navigation keys, editing keys, modifiers, screenshots, and media controls. The arrows are on the right home row in an inverted-T arrangement.

## Numbers

The number row follows the same left-to-right order as a Mac keyboard. The second row contains the corresponding Shift symbols, and the third row contains common brackets and punctuation.

```text
1 2 3 4 5 6        7 8 9 0 - =
! @ # $ % ^        & * ( ) _ +
` ~ [ ] { }        \ | , . / ?
```

## Symbols

Programming and punctuation symbols, including paired brackets, braces, parentheses, comparison operators, quotes, pipe, slash, and backslash.

## Function

F1-F12, system navigation, media and brightness controls. The outer bottom keys provide source-local bootloader/reset access for each half.

## Mouse

Hold the right inner Space thumb to activate the mouse layer. All left-half keys are disabled on this layer; only the right half controls the pointer.

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
