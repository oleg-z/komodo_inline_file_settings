### Komodo Inline File Settings

#### Original source
Most of the code was taken from this forum thread: http://community.activestate.com/forum/komode-modeline-support-komodo

#### Installation
* Enable macro side bar: View->Tabs & Sidebars->Toolbox
* Right click inside of side bar -> Import Package -> Import -> Choose komodo_inline_file_settings.kpz
* Macro is active now!

####Usage
  * Komodo settings  
    Add a line, like above (komode: params=go here). Must be either at the start of a line, or preceded by a whitespace character.  
    Komodo Parameters:
      * lineends|linends|le: Line ending format (should be autodetected, anyway)
      * language|syntax: Use this language for UDL parsing
      * codepage: file codepage/encoding. Use utf8. You know you want to.
      * tabwidth|tab: size of tab sharacters
      * tabs|notabs: don't expand (or do) tab characters
      * indentwidth: size of indents
  * Vim settings
    * fileformat
    * tabstop
    * noexpandtabs
    * expandtabs
    * shiftwidth
    * syntax
    * ts
  * Note: Komodo settings have a priority over 
  * Note2: if a tabwidth is set, but indentwidth is not, indentwidth assumes
    the value of tabwidth. This is probably what you want in the first place,
     but if it isn't, just set the indentwidth explicitly.
     
#### Examples
 * Komodo string:  
   ```komode: le=unix language=javascript codepage=utf8 tab=4 notabs indent=4```
 * Vim string:  
   ```vim:set ts=4 noexpandtabs:```
