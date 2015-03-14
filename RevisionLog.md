# revision history #

## Beta releases ##
<pre>
no beta release online<br>
</pre>

## Releases ##
### v 1.0.4 ([r156](https://code.google.com/p/cr-data-manager/source/detail?r=156)) ###
<pre>
fixed - error when assigning a Null value to numerical fields (issue 76)<br>
fixed - error message has meaningless line number (issue 77)<br>
fixed - user cannot cancel parsing a *very* large ruleset collection (issue 78)<br>
</pre>
### v 1.0.3 ([r155](https://code.google.com/p/cr-data-manager/source/detail?r=155)) ###
<pre>
fixed - cancellation of backgroundworker did not work as expected (issue 74)<br>
fixed - Data Manger won't run in a combined script after CV Scraper (issue 75)<br>
</pre>
### v 1.0.2 ([r154](https://code.google.com/p/cr-data-manager/source/detail?r=154)) ###
<pre>
change - GUI tab order corrected<br>
change - GUI supports import / export of groups<br>
change - GUI supports import option<br>
change - GUI: Text edit of Rulesets (in the ruleset panel) now always visible<br>
change - GUI: window is resizable<br>
change - included GUI 0.1.1r18<br>
</pre>

### v 1.0.1 ###
<pre>r152<br>
change - included GUI 0.1.1r11<br>
</pre>
<pre>r151<br>
change - added string fields BookAge,BookCondition,BookLocation to dataman.ini (issue 68)<br>
fixed - range modifiers GreaterEq etc. might give unexpected results (issue 71)<br>
fixed - progress form now supports cancellation while running over the selected books<br>
</pre>
### v 1.0.0 ###
<pre>
r150 (RC2)<br>
fixed - user.ini was overwritten by installation (issue 70, was missing in keepfiles parameter)<br>
fixed - Exception in stringRemoveLeading (str.startsWith() used instead of str.startswith() )<br>
change - includes GUI 0.1.1r10<br>
<br>
<br>
r149 (RC1)<br>
fixed - combination of numerical key and Null value like <<Count:>> raised Exception<br>
bug - if a large set of books is selected then the second progressbar will freeze<br>
fixed - if an Exception is thrown while executing the rules the for loop continues running<br>
change - using the backgroundWorker to handle the main loops<br>
fixed - erratic error: expecting an indented block (issue 66).<br>
Code now is written to memory, not to file as before<br>
change - includes GUI 0.1.0r8 RC9<br>
</pre>

### v 0.1.15 (last beta before 1.0, not public) ###
<pre>
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
...<br>
r125<br>
change - parser directive '#@ END_GROUP' added (issue 56)<br>
change - new list ruleFile.pseudoNumericalKeys (Number, AlternateNumber)<br>
change - new modifier Add for string type fields (non-multi value) (issue 32)<br>
change - new modifier Replace for string type fields (non-multi value) (issue 32)<br>
change - new modifier Remove for string type fields (non-multi value) (issue 32)<br>
fixed - range modifiers for multivalue keys are now restricted<br>
to the elements of ruleFile.allowedKeyModifiersMulti (issue 55)<br>
...<br>
r128<br>
change - new modifier NotStartsWith<br>
change - new modifier NotStartsWithAnyOf<br>
change - new value modifier RemoveLeading<br>
(leading and trailing blanks are respected) (issue 53)<br>
fixed - StringReplace modifier does not ignore leading or<br>
trailing blanks anymore<br>
change - added directives #@ AUTHOR, #@ NOTES, #@ END_NOTES (issue 59)<br>
change - added all missing fields of type string, numeric, multi-value<br>
change - when book was touched the process date is now written to CustomValue 'DataManager.processed'<br>
(this was it is only displayed when turned on with ShowCustomScriptValues = true in ComicRack.ini)<br>
...<br>
r129<br>
fixed - comparer >= etc. did not work as expected with numerical values<br>
fixed - progressbar was hidden behind CR window when clicked (removed MainWindow handle, issue 52)<br>
...<br>
r133<br>
change - allowed vals and modifiers are read from dataman.ini<br>
...<br>
r136<br>
change - integration of user.ini<br>
change - startup dialog asks user if he wants to start Data Manager running<br>
change - all dialog frames set to Fixed3D (fixes issue 13)<br>
...<br>
r138 TEST RELEASE<br>
change - configure runs GUI exe<br>
...<br>
r140<br>
fixed - string condition for numerical field throws exception (issue 61)<br>
fixed - the progressbar form is not disposed if parser code raises error<br>
change - added argument FOLDER to gui call<br>
fixed - exception when infinite symbol is used with number (issue 63)<br>
fixed - various problems with infinite symbol<br>
fixed - reading and writing the configuration with unicode characters from old gui raised Exception<br>
<br>
r141<br>
fixed - progressbar does not show progress while parsing rules<br>
fixed - label text of progressbar is not updating<br>
fixed - progressbar was not centered<br>
change - added allowedValModifiersNumeric to dataman.ini<br>
fixed - GUI crashes if called with path argument (issue 64, no path argument needed anymore)<br>
<br>
r142<br>
fixed - exception when min value in range is greater than max value<br>
fixed - exception with non-ASCII characters in string fields<br>
fixed - exception when a temporary file was locked<br>
<br>
r143<br>
change - new modifiers isAnyOf and NotIsAnyOf (included in dataman.ini) (issue 51)<br>
change - includes GUI 0.1.0r8 RC2<br>
<br>
r145<br>
fix - functions replace, remove, removeLeading now compare caseinsensitive<br>
change - includes GUI 0.1.0r8 RC6</pre>

### v 0.1.14 release 83 (last public release before 1.0) ###
<pre>
fixed - unexpected result if criteria in Number field is Null (issue 31)<br>
fixed - Null values in numerical fields are actually stored as -1 by CR. Using Null values in<br>
criteria on these field might return unexpected results<br>
fixed - exception if book.Number is Null and used in conjunction with ==, >, <, >=, <= etc.<br>
fixed - maximization of form displayResults was possible<br>
change - multiValueAdd rewritten to get rid of duplicates because of leading blanks etc.<br>
change - multiValueReplace rewritten to get rid of duplicates because of leading blanks etc.<br>
change - multiValueRemove rewritten to get rid of duplicates because of leading blanks etc.<br>
<br>
<br>
v 0.1.13 r72<br>
<br>
fixed - exception if generated code raises error<br>
fixed - exception if rules tries to set numerical field to zero value<br>
fixed - progress bar does not close if error in generated code<br>
<br>
v 0.1.12 r67<br>
<br>
fixed - colon in series results in #invalid expression<br>
fixed - error when running Data Manager if existing dataman.dat was in v 0.1.10 format<br>
<br>
v 0.1.11 r62<br>
<br>
change - function writeDataFile() rewritten to make it easier to read (and edit) with Notepad etc.<br>
change - configurator displays current line number<br>
change - cursor of configurator set to Cursors.Wait while saving data<br>
change - modifiers in keys and newvals are case tolerant (you may use StartsWith or startsWith or startswith)<br>
fix - exception if no double colon ':' in NewValue part of rule<br>
fix - exception if no double colon ':' in Criteria part of rule<br>
fix - slight delay when code was generated eliminated by removing debug code<br>
change - Genre field allowed<br>
change - Tags field allowed<br>
change - Add, Remove, Replace as modifiers for multi value fields<br>
change - Tag "DMProc" added if a book has been modified by Data Manager<br>
<br>
v 0.1.10 changes r53<br>
<br>
note written to log file if old value = new value (issue 18)<br>
unicode support added (issue 20)<br>
log viewer displays unicode correctly<br>
function writeCode rewritten<br>
<br>
#<br>
# v 0.1.9 r43<br>
# fixed: unexpected results if Calc modifier is used in rules<br>
#<br>
# v 0.1.8 r32 changes<br>
#<br>
# main dialog polished<br>
# new "About" dialog<br>
# class initialForm renamed to mainForm<br>
# info on log viewer if no book book was touched<br>
# text in configurator and log viewer is not pre-selected anymore<br>
# typos in aboutForm.label and mainForm.label corrected<br>
# close button added to log viewer<br>
# licence information integrated in code<br>
# status label in configurator if data was changed or saved<br>
# progress bar while rules are running<br>
# custom dialog instea of MessageBox to display result of running dataMan<br>
#<br>
# v 0.1.7 fixed<br>
# unexpected error writes 0 byte configuration<br>
# unexpected behavior if lines in configuration are prefixed before <<<br>
# due to syntax error FilePath is not considered a valid field<br>
#<br>
# v 0.1.7 changes<br>
# syntax check before configuratin is written<br>
# empty lines are excluded from configuration<br>
# configurator and init window set to fixed size<br>
# Genre can be used in criteria and new value part<br>
# configurator allows use of tabs<br>
# configurator does not use word wrap<br>
# design of configurator updated<br>
#<br>
# v 0.1.7 issues<br>
# tags field not included<br>
# initial dialog needs "about" button<br>
#<br>
# v 0.1.6 fixes<br>
# range modifier does not work as expected<br>
<br>
# v 0.1.5 fixes:<br>
# range modifier is mis-interpreted<br>
# problems for the number field with > >= < <=<br>
# minus entries in Number field are interpreted incorrectly<br>
# decimal value in number field throws exception<br>
<br>
# v 0.1.4 changes:<br>
# global use of configurator form (in progress)<br>
# added icons<br>
# added hook in toolbar<br>
# added initial form to run or configure<br>
# added LogFile viewer<br>
#<br>
# v 0.1.4 fixes:<br>
# exception thrown when StarsWith modifier was used with a second criterion<br>
<br>
v 0.1.3 changes:<br>
Format field can be used<br>
new modifier StartsWith<br>
AlternateSeries can be used<br>
field Count can be used<br>
fields FilePath and FileName can be used<br>
configuration file can be edited from within ComicRack<br>
<br>
v 0.1.3 fixes:<br>
exception thrown if dataman.dat does not exist<br>
<br>
v 0.1.2 fixes:<br>
exception because of missing newline after criteria<br>
Range modifier was misinterpreted if the field is non-numerical (like Number)<br>
<br>
v.0.1.1 changes:<br>
generated code includes exception handling<br>
<br>
v 0.1.0 changes:<br>
read configuration from replacaData.dat - done 2013-03-13<br>
added 'Contains' as modifier (e.g. <<FileDirectory.Contains:TPB>> => <<Format:TPB>>)<br>
more modifiers: Greater, GreaterEq, Less, LessEq<br>
use of FileDirectory allowed in criteria<br>
use of SeriesGroup allowed in criteria and newVals<br>
use of MainCharacterOrTeam is allowed in criteria and newVals<br>
parser errors are written to replaceData.log<br>
added Calc as modifier in newValue (e.g. => <<Number:{Number} - 441>>)<br>
results are logged in file replaceData.log<br>
<br>
v 0.1.0 fixes:<br>
Exception thrown when you try to insert a string value in a numerical field<br>
<br>
<br>
</pre>