![Addon Logo](https://cdn.discordapp.com/attachments/439457786129285120/642313410368766025/GDAddonLogo_001-hd.png)

# GD Addon SDK

SDK for modules development

### Consists of
* GDAPI _(cocos2d-x, GD classes and custom extensions)_
* ImGui _(dear imgui | [GitHub](http://github.com/ocornut/imgui))_
* EX _(additional classes/functions)_


## Example
```cpp
#include "GDAModule.h"
#include "EXLog.h"
GDA_MODULE_CALLBACK(GDA_MODULE *pModule) {
    pModule->setName("Example");
    pModule->setAuthor("a man");
    pModule->registerClickCallback(CALLBACK_L(void, GDA_MODULE *pModule) {
        static int counter = 1;
        EXLog("Counter = %d", counter++);
    });
    return true;
}
```

## Progress

GDAPI:
▰▰▰▰▰▰▱▱▱▱▱▱▱▱▱▱▱▱▱▱ (30%)

GDA SDK:
▰▰▰▰▰▰▰▰▰▰▰▰▰▰▱▱▱▱▱▱ (70%)



> *GD Addon has been in development since 19 July 2018*
