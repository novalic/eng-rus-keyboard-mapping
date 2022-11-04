# English - Russian keyboard mapping

This is my custom mapping for russian alphabet in my english keyboard in Ubuntu.
I did this to avoid buying keyboard stickers for the usual Russian keyboard layout while I was learning Russian language.


## How to install

_Ubuntu 20.04.4 LTS_

1) Copy the file `rc` to the directory `/usr/share/X11/xkb/symbols`
   _) sudo cp rc /usr/share/X11/xkb/symbols/
2) Edit the file `/usr/share/X11/xkb/rules/evdev.xml`:
   _i) Find the section layoutList.
   _ii) Add the following:
    ```xml
    <layout>
      <configItem>
        <name>rc</name>
        <shortDescription>rc</shortDescription>
        <description>RussianCustom</description>
        <languageList>
          <iso639Id>cod</iso639Id>
        </languageList>
      </configItem>
      <variantList>
      </variantList>
    </layout>
   ```
3) In Settings - Keyboard:
   _i) Click + to add a new input source
   _ii) Select the three falling dots and type Russian, the option "Other" will appear, select it.
   _iii) Type RussianCustom, select it and click Add.
   
## Mapping

![Mapping](mapping.png)
