Status: 0.1.15 [r121](https://code.google.com/p/cr-data-manager/source/detail?r=121)
# Major changes and fixes relevant to GUI #

v 0.1.15


&lt;PRE&gt;


change - PageCount added to allowed keys
change - new modifier ContainsAnyOf ([issue 28](https://code.google.com/p/cr-data-manager/issues/detail?id=28))
change - new modifier ContainsNot
change - new modifier ContainsAllOf ([issue 40](https://code.google.com/p/cr-data-manager/issues/detail?id=40))
change - new modifier NotContainsAnyOf
change - new modifier StartsWithAnyOf
change - new directive "#@ END\_RULES"
change - new directive #@ GROUP
change - new allowed fields: alternateNumber and alternateCount ([issue 44](https://code.google.com/p/cr-data-manager/issues/detail?id=44))
change - new allowed fields: Title
change - range modifier is not selectable for string fields anymore in GUI


Unknown end tag for &lt;/pre&gt;



## Complete listing of revisions ##
<pre>
v 0.1.15<br>
fixed - "do you want to see the log" dialogbox always appears behind the Comicrack Window<br>
(issue 34) (set ComicRack.Window  as parent window handle for all forms)<br>
change - modular rewriting of forms<br>
change - Contains compares now case insensitive<br>
change - StartsWith compares now case insensitive<br>
change - comparison for equality (==) is now case insensitive<br>
change - comparison for less (<) is now case insensitive<br>
change - comparison for lessEqual (<=) is now case insensitive<br>
change - comparison for greater (>) is now case insensitive<br>
change - comparison for greaterEq (>=) is now case insensitive<br>
change - comparison for not equal (<>) is now case insensitive<br>
fix - missing references to globalvars added<br>
change - PageCount added to allowed keys<br>
change - new modifier ContainsAnyOf (issue 28)<br>
change - new modifier ContainsNot (may used as well as NotContains)<br>
change - new modifier ContainsAllOf (issue 40)<br>
change - if no value was modified by the DM, only "book xxx was touched" is written to logfile<br>
change - new modifier NotContainsAnyOf<br>
change - new modifier StartsWithAnyOf<br>
change - new directive "#@ END_RULES"<br>
change - new class "parser"<br>
change - new class "ruleFile" (encapsulated reading and writing the DATFILE)<br>
fix - exception when Null value was used in Range modifier<br>
change - when error was raised by compiling code a MessageBox will show the error<br>
...<br>
r105<br>
change - Configurator form re-written<br>
change - basic Search functionality in Configurator<br>
...<br>
r106<br>
change - first rudimentary GUI written (no functionality yet)<br>
...<br>
r109<br>
change - ComicRack version check at start (min is 0.9.165)<br>
change - basic GUI functionality<br>
...<br>
r111<br>
change - new directive #@ GROUP<br>
change - added combobox to find group header in textbox<br>
change - textclips (like commentary line, group header etc. can be added via GUI)<br>
change - rule editor position set to CenterParent<br>
fixed - 'setvalue' was not recognized as a valid modifier<br>
fixed - exception if file in rule editor is not the DatFile and combobox group selector is selected<br>
...<br>
r113<br>
fixed - sometimes selected text in rule set is overwritten by inserted rule (GUI)<br>
fixed - criterion or setvalue are not added to rule if already in there (GUI)<br>
change - buttons for deleting content of textboxes for criteria and setvalue (GUI)<br>
change - group names are checked if already used<br>
fixed - Contains... methods in class parser rewritten (unexpected results when leading<br>
or trailing blanks where attached to values)<br>
fixed - exception when a criterion with apostrophe or quotation mark was written to the log file<br>
(issue 36)<br>
...<br>
r114<br>
change - save and close added to configurator menustrip<br>
change - option to backup and restore the rule set (issue 30)<br>
change - DMProc is no longer added to Tags but written as a custom value (issue 33)<br>
..<br>
r115<br>
change - new allowed fields: alternateNumber and alternateCount (issue 44)<br>
fixed - comboModifiers does not match comboCriteria and comboValues (issue 48)<br>
change - option to select line by line number (issue 49)<br>
...<br>
r117<br>
change - GUI: delete rule from rule set<br>
change - GUI: re-engineer rule<br>
change - menu strip upgraded<br>
...<br>
r121<br>
change - new allowed fields: Title<br>
fixed - unexpected behavior with book numbers like '5AU', 'Minus 1', '¼', fixed with<br>
function 'stringToFloat'<br>
change - rule editor is now dropdown option in CR toolbar (form MainForm is obsolete)<br>
change - range modifier is not selectable for string fields anymore in GUI<br>
fixed - group header combo box was not updated when backup of rule set was loaded<br>
</pre>