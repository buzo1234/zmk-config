# Piantor Pico 2 keymap

The production firmware is a wired, full-duplex ZMK split. The left half is the only central and the only half intended to connect to the host over USB. The right half is a peripheral.

The four middle thumb keys are layer-taps: tap for their normal key and hold for the named layer.

```text
Left GUI | Backspace/Nav | Space/Numbers     Space/Symbols | Enter/Function | Right Alt
```

## Base

```text
Tab   Q W E R T        Y U I O P Backspace
Ctrl  A S D F G        H J K L ; '
Shift Z X C V B        N M , . / Shift
          GUI Backspace Space    Space Enter Alt
```

## Navigation

Navigation keys, editing keys, modifiers, screenshots, and media controls. The arrows are on the right home row in an inverted-T arrangement.

## Numbers

A right-hand number pad plus brackets and common arithmetic operators. Zero, decimal point, and Enter are on the right thumbs.

## Symbols

Programming and punctuation symbols, including paired brackets, braces, parentheses, comparison operators, quotes, pipe, slash, and backslash.

## Function

F1-F12, system navigation, media and brightness controls. The outer bottom keys provide source-local bootloader/reset access for each half.

## Flashing and cable safety

- Flash `piantor_pico2_left.uf2` to the left half.
- Flash `piantor_pico2_right.uf2` to the right half.
- Power the completed keyboard from the left half only.
- Never insert or remove the TRRS cable while either half is powered.
