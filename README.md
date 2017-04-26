# mbed_memap
Using memap.py that is a mbed tool for show details information when compile project (*.map file)
- Flash
- RAM
- Heap, stack
- Modules in your app
- ....

## Resources
- Tool: https://github.com/ARMmbed/mbed-os/blob/master/tools/memap.py (`git clone https://github.com/ARMmbed/mbed-os.get`)
- Instruction: https://github.com/ARMmbed/mbed-os/blob/mbed-os-5.2/docs/memap.md (`Important`)

## Command
- Example: `python memap.py example.map -t GCC_ARM -o memap_result.txt -e table`

## *.map file for GCC compiler
- Create map file after compile project
Add the follow option to Linker flags (LD_FLAGS)
`-Wl,-Map=$(PROJECT).map`

## Enjoy
- From the results which is showed from memap.py you can modif:
    + Compile config for reduce application size
    + Heap, Stack size config in linker file (ex: NRF51822.LD)




