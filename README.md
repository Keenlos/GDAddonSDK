![Addon Logo](https://cdn.discordapp.com/attachments/439457786129285120/642313410368766025/GDAddonLogo_001-hd.png)

# GD Addon SDK

Source Development Kit to modules developing

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
    pModule->setClickCallback(CALLBACK_L(void, GDA_MODULE *pModule) {
        static int counter = 1;
        EXLog("Counter = %d", counter++);
    });
    return true;
}
```
![The module](https://cdn.discordapp.com/attachments/491677291588616213/643430791677870101/c.PNG)
![The module](https://cdn.discordapp.com/attachments/491677291588616213/643430824301297667/55d82c92e13bbf6a.PNG)

## Progress

GDAPI:
▰▰▰▰▰▰▱▱▱▱▱▱▱▱▱▱▱▱▱▱ (30%)

GDA SDK:
▰▰▰▰▰▰▰▰▰▰▰▰▰▰▱▱▱▱▱▱ (70%)



> *GD Addon has been in development since 19 July 2018*
