# MySensors_SI7021



## Introduction

This is an attempt to make it easy to resolve a common problem when people first get started with using the 'MySensors Sensebender Micro' board.  A lightweight, custom modified library is referenced and available within the [MySensorsArduinoExamples](/mysensors/MySensorsArduinoExamples) repository but it's not a user friendly method of distributing the library.  This project is my attempt to rectify that.

This project is [ready to be sumitted](https://github.com/arduino/library-registry/blob/main/FAQ.md#submission-requirements) to [Arduino Library Registry](https://github.com/arduino/library-registry) index making it available to install directly through the Library Manager in the Arduino IDE, Arduino CLI, PlatformIO, etc.  It just needs to be submitted[^1]. At some point in the future, I'd like to have this project adopted into the MySensors group of repositories and submitted to Library Manager from there.  

---

## How to use this library

Until the library is available to add to your project through the Library Manager, you'll need to install it manually.  Here's how to do that.

```bash
cd ~/Arduino/libraries
```

```bash
git clone https://github.com/AlphaSierraHotel/MySensors_SI7021.git
```

Then change the references in the sketches to match the new library name.  Change references of `#include <SI7021.h>` to be `<MySensors_SI7021.h>`.

For example, in your code, change this:

```cpp
#include <MySensors.h>
#include <Wire.h>
#include <SI7021.h>
```

to this:

```cpp
#include <MySensors.h>
#include <Wire.h>
// #include <SI7021.h>
#include <MySensors_SI7021.h>
```

That's it, try compiling the code.

---

## Foot Notes

[^1]:
    See [adding a library to Library Manager](https://github.com/arduino/library-registry#adding-a-library-to-library-manager)
    See also, [Arduino Library Manager FAW](https://github.com/arduino/library-registry/blob/main/FAQ.md#arduino-library-manager-faq)

The repository must have a Git tag or GitHub release.
