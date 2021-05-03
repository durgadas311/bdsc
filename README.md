# bdsc
## BD Software C Compiler

This repo exists mainly to fix problems or bugs with BDSC.

First problem fixed: BDSC failed on CP/NET or any system where the CCP
was not the original size of 2K. The fix is to disable BDSC attempts
to detect CCP overrun and never return directly to the CCP - always warm boot.
