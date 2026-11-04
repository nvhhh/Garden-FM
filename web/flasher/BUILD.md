# Felucca build from main, 2ebd564

- Source: nvhhh/garden-fm, branch `main`, commit `2ebd564` ("GEN: MELODIC above 50 no longer wraps the lead's repeat weight"; includes the MELODIC fix).
- Built with `./build.sh` (default options, no `--release`), JieLi toolchain jieli-linux-toolchains-20260730.1 and AC79 SDK AC79NN_SDK_V1.2.1_2023-12-13.
- Package identity: FM-1_900. Files: `felucca.fwsc` (installable package), `felucca.bin` (app image), `SHA256SUMS`.

## Usage

- Flash: 571,332 B used of the 584,336 B app slot, 13,004 B free.
- RAM: .data + .bss 94,916 B of 98,304 B (3,388 B free); RAM code 20,380 B of 25,600 B.
- Build checks: all passed (`ok` on image, RAM code and register access). One compiler warning (`-Wcomment` in `firmware/src/ui_monk.h`, cosmetic).

Not included: `loader/ota.bin` (6,957 B), which is inside the `.fwsc`.
