# NES-replay-files

These files sync using the TAStm32 replay device on a front loading NES from power on.
Unless otherwise noted below, use --blank 1

Additionally, the following runs require RAM cleared to the pattern used by default in FCEUX / BizHawk: Monopoly (both runs), Marble Madness, Rad Racer, Silver Surfer. Some games that require RAM clearing require a start from reset as RAM is too volatile, for these cases use --blank 0.

Metroid low percent requires the following command:
py -3 python\tastm32.py --console nes --players 1,5 --blank 0 --dpcm metroid_frame.r08
