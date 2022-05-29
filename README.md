# tuxsplit
Platform agnostic image based autosplitter (written in rust?)

## Feature Goals
- [ ] image based autosplitting
- [ ] memory state autosplitting for emulator
- [ ] hooking in to obs for video input
- [ ] gui configurator

## General program outline
1. console/emulator -video-> obs
2. obs plugin limited to minimum required area -video-> autosplit receiver
3. autosplit looks for predefined image in video feed
   - if image found: split
   - if image not found: do nothing
