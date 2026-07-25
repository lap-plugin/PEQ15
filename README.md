lap-PEQ15 — five-band parametric equaliser

A component-accurate circuit model of the Czechoslovak studio equaliser
“Parametric equaliser PEQ15”

lap PEQ15 is not an emulation tuned by ear. The audio you hear is computed by
a nodal circuit solver directly from the verified schematic of the original
hardware — every resistor, capacitor, potentiometer taper and op-amp of the
signal path is in the model. Turning a knob does not switch a digital filter;
it literally moves the potentiometer inside the simulated circuit, with the
capacitor states carried over — so sweeps behave exactly like on the real desk.

Sound & features

- 5 fully parametric bands with 100 % overlap — each band sweeps
  10 Hz–20 kHz in three ranges (×0.1 / ×1 / ×10), gain +12/−15 dB,
  bandwidth 0.03–2 octaves. Bands are grouped (1·3·5 / 2·4) exactly like the
  2006 re-edition to minimise interaction between neighbours.
- Input & output level ±12 dB with the original, measured non-linear
  potentiometer laws — the knobs respond like the hardware, not like a fader.
- Sweepable high-pass (10–250 Hz) and low-pass (3–40 kHz), 12 dB/oct
  Butterworth, built to the block specification of the 2006 re-edition.
- Balanced I/O board in the signal path (switchable): the instrument’s
  input receiver and the cross-coupled floating output driver, including their
  subtle low-end character.
- NJM4580 op-amp model (switchable to ideal): finite gain-bandwidth of the
  original chips, audible as a gentle high-frequency Q-enhancement.
- True stereo: two complete channel strips (L/R) with a LINK switch —
  linked they behave as one instrument, unlinked each side has its own EQ,
  filters and bypass. Mono configuration is available too.
- Oversampling 1× / 2× / 4× to keep the top octave tuning accurate at any
  session sample rate.
- SIMD-accelerated engine the solver auto-selects SSE2 / AVX2 / AVX-512
  at run time; the active instruction set is shown on the panel.
- Preset system portable `.peqpreset` files (SAVE/LOAD on the panel),
  independent of the DAW session state.
- Resizable hardware-style GUI a 19″ 2U stereo rack panel; drag the
  corner to scale the whole panel. Values appear when you touch a control.

Controls (per channel strip)

| Control | Function |
|---|---|
| INPUT / OUTPUT | level trims, ±12 dB (double-click = 0 dB) |
| HP / LP | sweepable high-pass 10–250 Hz and low-pass 3–40 kHz |
| FLT | inserts the HP/LP filters into the path |
| BYP | bypasses this channel |
| BAND 1–5: GAIN | +12/−15 dB (double-click = 0 dB) |
| BAND 1–5: FREQ·WIDE | one knob, FRQ/WIDE selector chooses what it tunes |
| BAND 1–5: RANGE | frequency range ×0.1 / ×1 / ×10 |
| BAND 1–5: ON | engages the band |
| LINK / L·R | links both strips or splits them into independent L and R |
| OS | oversampling 1× / 2× / 4× |
| SAVE / LOAD | preset manager |


