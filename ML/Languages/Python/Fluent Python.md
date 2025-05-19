---
annotation-target: prejohned/Fluent Python.pdf
---


>%%
>```annotation-json
>{"created":"2025-05-04T20:29:55.680Z","text":"Resources:\nhttps://fpy.li/code - Github of code ran\nhttps://www.fluentpython.com/ - general page ","updated":"2025-05-04T20:29:55.680Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^1cpf9gkq5dx|show annotation]]
>%%COMMENT%%
>Resources:
>https://fpy.li/code - Github of code ran
>https://www.fluentpython.com/ - general page 
>%%TAGS%%
>
^1cpf9gkq5dx


>%%
>```annotation-json
>{"created":"2025-05-04T20:31:18.687Z","updated":"2025-05-04T20:31:18.687Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":87379,"end":87501},{"type":"TextQuoteSelector","exact":" The Python interpreter invokes special methods to perform basic objectoperations,  often  triggered  by  special  syntax.","prefix":" Data Model to buildnew classes.","suffix":"  The  special  method  names  a"}]}]}
>```
>%%
>*%%PREFIX%%Data Model to buildnew classes.%%HIGHLIGHT%% ==The Python interpreter invokes special methods to perform basic objectoperations,  often  triggered  by  special  syntax.== %%POSTFIX%%The  special  method  names  a*
>%%LINK%%[[#^0zd0q9bn7gfr|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^0zd0q9bn7gfr


>%%
>```annotation-json
>{"created":"2025-05-04T20:31:31.007Z","text":"special method \\__getitem__ used to access a datamember of my_collection","updated":"2025-05-04T20:31:31.007Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":87621,"end":87781},{"type":"TextQuoteSelector","exact":"obj[key]  is  supported  by  the  __getitem__  special  method.  In  order  to  evaluatemy_collection[key], the interpreter calls my_collection.__getitem__(key)","prefix":"scores. For example, the syntax3","suffix":".We  implement  special  methods"}]}]}
>```
>%%
>*%%PREFIX%%scores. For example, the syntax3%%HIGHLIGHT%% ==obj[key]  is  supported  by  the  __getitem__  special  method.  In  order  to  evaluatemy_collection[key], the interpreter calls my_collection.__getitem__(key)== %%POSTFIX%%.We  implement  special  methods*
>%%LINK%%[[#^t2t1jnqxjz|show annotation]]
>%%COMMENT%%
>special method \__getitem__ used to access a datamember of my_collection
>%%TAGS%%
>
^t2t1jnqxjz


>%%
>```annotation-json
>{"created":"2025-05-04T20:37:12.324Z","text":"using special methods allows for easy syntax handling, notably using other libraries for the same tasks without performing it ourselves","updated":"2025-05-04T20:37:12.324Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":91608,"end":91809},{"type":"TextQuoteSelector","exact":"Should  we  create  a  method  to  pick  a  random  card?  No  need.  Python  already  has  afunction  to  get  a  random  item  from  a  sequence:  random.choice.  We  can  use  it  on  adeck instance","prefix":"-1]Card(rank='A', suit='hearts')","suffix":":>>> from random import choice>>"}]}]}
>```
>%%
>*%%PREFIX%%-1]Card(rank='A', suit='hearts')%%HIGHLIGHT%% ==Should  we  create  a  method  to  pick  a  random  card?  No  need.  Python  already  has  afunction  to  get  a  random  item  from  a  sequence:  random.choice.  We  can  use  it  on  adeck instance== %%POSTFIX%%:>>> from random import choice>>*
>%%LINK%%[[#^9u4brvjllhb|show annotation]]
>%%COMMENT%%
>using special methods allows for easy syntax handling, notably using other libraries for the same tasks without performing it ourselves
>%%TAGS%%
>
^9u4brvjllhb


>%%
>```annotation-json
>{"created":"2025-05-04T20:38:50.746Z","text":"\\__getitem__ does everything that [] can do, so slicing, iteration is available\n","updated":"2025-05-04T20:38:50.746Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":92385,"end":92506},{"type":"TextQuoteSelector","exact":"Because  our  __getitem__  delegates  to  the  []  operator  of  self._cards,  our  deckautomatically  supports  slicing.","prefix":"ice function.But it gets better.","suffix":"  Here’s  how  we  look  at  the"}]}]}
>```
>%%
>*%%PREFIX%%ice function.But it gets better.%%HIGHLIGHT%% ==Because  our  __getitem__  delegates  to  the  []  operator  of  self._cards,  our  deckautomatically  supports  slicing.== %%POSTFIX%%Here’s  how  we  look  at  the*
>%%LINK%%[[#^n9z9xulvl8c|show annotation]]
>%%COMMENT%%
>\__getitem__ does everything that [] can do, so slicing, iteration is available
>
>%%TAGS%%
>
^n9z9xulvl8c


>%%
>```annotation-json
>{"created":"2025-05-04T20:51:37.048Z","text":"!r in {self.value!r} makes sure that the value is kept as is and not represented as a string","updated":"2025-05-04T20:51:37.048Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":102532,"end":102886},{"type":"TextQuoteSelector","exact":"Note  that  the  f-string  in  our  __repr__  uses  !r  to  get  the  standard  representation  ofthe attributes to be displayed. This is good practice, because it shows the crucial dif‐ference between Vector(1, 2) and Vector('1', '2')—the latter would not work inthe context of this example, because the constructor’s arguments should be numbers,not str","prefix":"-strings  the  str.formatmethod.","suffix":".12 | Chapter 1: The Python Data"}]}]}
>```
>%%
>*%%PREFIX%%-strings  the  str.formatmethod.%%HIGHLIGHT%% ==Note  that  the  f-string  in  our  __repr__  uses  !r  to  get  the  standard  representation  ofthe attributes to be displayed. This is good practice, because it shows the crucial dif‐ference between Vector(1, 2) and Vector('1', '2')—the latter would not work inthe context of this example, because the constructor’s arguments should be numbers,not str== %%POSTFIX%%.12 | Chapter 1: The Python Data*
>%%LINK%%[[#^qelijno7jcr|show annotation]]
>%%COMMENT%%
>!r in {self.value!r} makes sure that the value is kept as is and not represented as a string
>%%TAGS%%
>
^qelijno7jcr


>%%
>```annotation-json
>{"created":"2025-05-04T20:54:45.000Z","text":"generally \\__repr\\__ and \\__str\\__ are the same, but \\__repr\\__ should explictly be the string representation of the exact object ","updated":"2025-05-04T20:54:45.000Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":103351,"end":103631},{"type":"TextQuoteSelector","exact":"Sometimes same string returned by __repr__ is user-friendly, and you don’t need tocode  __str__  because  the  implementation  inherited  from  the  object  class  calls__repr__  as  a  fallback.  Example  5-2  is  one  of  several  examples  in  this  book  with  acustom __str__","prefix":"itable for display to end users.","suffix":".Programmers  with  prior  exper"}]}]}
>```
>%%
>*%%PREFIX%%itable for display to end users.%%HIGHLIGHT%% ==Sometimes same string returned by __repr__ is user-friendly, and you don’t need tocode  __str__  because  the  implementation  inherited  from  the  object  class  calls__repr__  as  a  fallback.  Example  5-2  is  one  of  several  examples  in  this  book  with  acustom __str__== %%POSTFIX%%.Programmers  with  prior  exper*
>%%LINK%%[[#^6yf46uzctlc|show annotation]]
>%%COMMENT%%
>generally \__repr\__ and \__str\__ are the same, but \__repr\__ should explictly be the string representation of the exact object 
>%%TAGS%%
>
^6yf46uzctlc


>%%
>```annotation-json
>{"created":"2025-05-04T20:56:07.986Z","text":"check if x\\.__bool\\__() is implemented and get boolean value that way, else use x.\\__len\\__()\n","updated":"2025-05-04T20:56:07.986Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":104326,"end":104652},{"type":"TextQuoteSelector","exact":"By  default,  instances  of  user-defined  classes  are  considered  truthy,  unless  either__bool__ or __len__ is implemented. Basically, bool(x) calls x.__bool__() and usesthe result. If __bool__ is not implemented, Python tries to invoke x.__len__(), andif that returns zero, bool returns False. Otherwise bool returns True","prefix":"ichreturns either True or False.","suffix":".Our implementation of __bool__ "}]}]}
>```
>%%
>*%%PREFIX%%ichreturns either True or False.%%HIGHLIGHT%% ==By  default,  instances  of  user-defined  classes  are  considered  truthy,  unless  either__bool__ or __len__ is implemented. Basically, bool(x) calls x.__bool__() and usesthe result. If __bool__ is not implemented, Python tries to invoke x.__len__(), andif that returns zero, bool returns False. Otherwise bool returns True== %%POSTFIX%%.Our implementation of __bool__*
>%%LINK%%[[#^wsn75irzmn|show annotation]]
>%%COMMENT%%
>check if x\.__bool\__() is implemented and get boolean value that way, else use x.\__len\__()
>
>%%TAGS%%
>
^wsn75irzmn


>%%
>```annotation-json
>{"created":"2025-05-04T20:58:15.591Z","text":"UML of the Abstract Base Classes from collections.abc module.\n\nEach title is called the interface and it has a set of special methods to perform to be implemented","updated":"2025-05-04T20:58:15.591Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":106040,"end":106303},{"type":"TextQuoteSelector","exact":"Figure 1-2. UML class diagram with fundamental collection types. Method names initalic are abstract, so they must be implemented by concrete subclasses such as listand dict. The remaining methods have concrete implementations, therefore subclassescan inherit them","prefix":" are built from special methods.","suffix":".Each  of  the  top  ABCs  has  "}]}]}
>```
>%%
>*%%PREFIX%%are built from special methods.%%HIGHLIGHT%% ==Figure 1-2. UML class diagram with fundamental collection types. Method names initalic are abstract, so they must be implemented by concrete subclasses such as listand dict. The remaining methods have concrete implementations, therefore subclassescan inherit them== %%POSTFIX%%.Each  of  the  top  ABCs  has*
>%%LINK%%[[#^lus3ropslfp|show annotation]]
>%%COMMENT%%
>UML of the Abstract Base Classes from collections.abc module.
>
>Each title is called the interface and it has a set of special methods to perform to be implemented
>%%TAGS%%
>
^lus3ropslfp


>%%
>```annotation-json
>{"created":"2025-05-04T20:59:54.492Z","text":" ","updated":"2025-05-04T20:59:54.492Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":108437,"end":108489},{"type":"TextQuoteSelector","exact":"Table 1-1. Special method names (operators excluded)","prefix":"Overview of Special Methods | 15","suffix":"Category Method namesString/byte"}]}]}
>```
>%%
>*%%PREFIX%%Overview of Special Methods | 15%%HIGHLIGHT%% ==Table 1-1. Special method names (operators excluded)== %%POSTFIX%%Category Method namesString/byte*
>%%LINK%%[[#^eu9rcplpae|show annotation]]
>%%COMMENT%%
> 
>%%TAGS%%
>
^eu9rcplpae


>%%
>```annotation-json
>{"created":"2025-05-04T21:40:38.504Z","updated":"2025-05-04T21:40:38.504Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":109591,"end":109648},{"type":"TextQuoteSelector","exact":"Table 1-2. Special method names and symbols for operators","prefix":"ion, as we’ll see in Chapter 16.","suffix":"Operator category Symbols Method"}]}]}
>```
>%%
>*%%PREFIX%%ion, as we’ll see in Chapter 16.%%HIGHLIGHT%% ==Table 1-2. Special method names and symbols for operators== %%POSTFIX%%Operator category Symbols Method*
>%%LINK%%[[#^6gtzctznd6|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^6gtzctznd6


>%%
>```annotation-json
>{"created":"2025-05-04T21:47:42.075Z","text":"different types of sequences, Ones that hold multiple types and ones that hold 1 type.\n\nContainer sequences holds refernces, while flat sequences hold it own contents in memory","updated":"2025-05-04T21:47:42.075Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":121644,"end":121873},{"type":"TextQuoteSelector","exact":"Container sequencesCan  hold  items  of  different  types,  including  nested  containers.  Some  examples:list, tuple, and collections.deque.Flat sequencesHold items of one simple type. Some examples: str, bytes, and array.array","prefix":"sequence types implemented in C:","suffix":".22 | Chapter 2: An Array of Seq"}]}]}
>```
>%%
>*%%PREFIX%%sequence types implemented in C:%%HIGHLIGHT%% ==Container sequencesCan  hold  items  of  different  types,  including  nested  containers.  Some  examples:list, tuple, and collections.deque.Flat sequencesHold items of one simple type. Some examples: str, bytes, and array.array== %%POSTFIX%%.22 | Chapter 2: An Array of Seq*
>%%LINK%%[[#^r7hzcjgvwif|show annotation]]
>%%COMMENT%%
>different types of sequences, Ones that hold multiple types and ones that hold 1 type.
>
>Container sequences holds refernces, while flat sequences hold it own contents in memory
>%%TAGS%%
>
^r7hzcjgvwif


>%%
>```annotation-json
>{"created":"2025-05-04T21:49:24.672Z","text":"arrays (flat sequence) of primatives is much smaller than tuples (container sequence) because of the metadata","updated":"2025-05-04T21:49:24.672Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":122996,"end":123306},{"type":"TextQuoteSelector","exact":"On a 64-bit Python build, each of those fields takes 8 bytes. That’swhy an array of floats is much more compact than a tuple of floats:the  array  is  a  single  object  holding  the  raw  values  of  the  floats,while the tuple consists of several objects—the tuple itself and eachfloat object contained in it","prefix":"e holding the value of the float","suffix":".Overview of Built-In Sequences "}]}]}
>```
>%%
>*%%PREFIX%%e holding the value of the float%%HIGHLIGHT%% ==On a 64-bit Python build, each of those fields takes 8 bytes. That’swhy an array of floats is much more compact than a tuple of floats:the  array  is  a  single  object  holding  the  raw  values  of  the  floats,while the tuple consists of several objects—the tuple itself and eachfloat object contained in it== %%POSTFIX%%.Overview of Built-In Sequences*
>%%LINK%%[[#^dqz5szrno6m|show annotation]]
>%%COMMENT%%
>arrays (flat sequence) of primatives is much smaller than tuples (container sequence) because of the metadata
>%%TAGS%%
>
^dqz5szrno6m


>%%
>```annotation-json
>{"created":"2025-05-04T21:52:12.672Z","text":"mutable: elements can be changed within\nunmutable: elements cannot be changed ","updated":"2025-05-04T21:52:12.672Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":123342,"end":123398},{"type":"TextQuoteSelector","exact":"Another way of grouping sequence types is by mutability:","prefix":"rview of Built-In Sequences | 23","suffix":"Mutable sequencesFor example, li"}]}]}
>```
>%%
>*%%PREFIX%%rview of Built-In Sequences | 23%%HIGHLIGHT%% ==Another way of grouping sequence types is by mutability:== %%POSTFIX%%Mutable sequencesFor example, li*
>%%LINK%%[[#^mts55fuo36f|show annotation]]
>%%COMMENT%%
>mutable: elements can be changed within
>unmutable: elements cannot be changed 
>%%TAGS%%
>
^mts55fuo36f


>%%
>```annotation-json
>{"created":"2025-05-04T22:00:25.591Z","text":"do list comprehension when possible to avoid further reading for the same amount of understanding\n","updated":"2025-05-04T22:00:25.591Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":126351,"end":126655},{"type":"TextQuoteSelector","exact":"A for loop may be used to do lots of different things: scanning a sequence to count orpick  items,  computing  aggregates  (sums,  averages),  or  any  number  of  other  tasks.The code in Example 2-1 is building up a list. In contrast, a listcomp is more explicit.Its goal is always to build a new list.","prefix":"ecause  its  intent  isexplicit.","suffix":"List Comprehensions and Generato"}]}]}
>```
>%%
>*%%PREFIX%%ecause  its  intent  isexplicit.%%HIGHLIGHT%% ==A for loop may be used to do lots of different things: scanning a sequence to count orpick  items,  computing  aggregates  (sums,  averages),  or  any  number  of  other  tasks.The code in Example 2-1 is building up a list. In contrast, a listcomp is more explicit.Its goal is always to build a new list.== %%POSTFIX%%List Comprehensions and Generato*
>%%LINK%%[[#^ww3m7oj46ul|show annotation]]
>%%COMMENT%%
>do list comprehension when possible to avoid further reading for the same amount of understanding
>
>%%TAGS%%
>
^ww3m7oj46ul


>%%
>```annotation-json
>{"created":"2025-05-04T22:02:32.317Z","text":"walrus operator (:=) can be used evaluate and save the value:\n\nie we avoid using len(a) twice:\n```python\nif (n := len(a)) > 10:\n    print(f\"List is too long ({n} elements, expected <= 10)\")\n```","updated":"2025-05-04T22:02:32.317Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":128418,"end":128548},{"type":"TextQuoteSelector","exact":"defines the scope of the target of := as the enclos‐ing function, unless there is a global or nonlocal declaration for that target","prefix":".PEP 572—Assignment Expressions ","suffix":".2>>> x = 'ABC'>>> codes = [ord("}]}]}
>```
>%%
>*%%PREFIX%%.PEP 572—Assignment Expressions%%HIGHLIGHT%% ==defines the scope of the target of := as the enclos‐ing function, unless there is a global or nonlocal declaration for that target== %%POSTFIX%%.2>>> x = 'ABC'>>> codes = [ord(*
>%%LINK%%[[#^3vd0yeblt4n|show annotation]]
>%%COMMENT%%
>walrus operator (:=) can be used evaluate and save the value:
>
>ie we avoid using len(a) twice:
>```python
>if (n := len(a)) > 10:
>    print(f"List is too long ({n} elements, expected <= 10)")
>```
>%%TAGS%%
>
^3vd0yeblt4n


>%%
>```annotation-json
>{"created":"2025-05-04T22:16:09.783Z","text":"genexp are generally better because it yields to give 1 item at a time, while list comprehension feeds the whole list and all elements into at once\n\ngenexp are preformed the same as list comp, but with ()","updated":"2025-05-04T22:16:09.783Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":132582,"end":132777},{"type":"TextQuoteSelector","exact":"a  genexp  (generator  expression)  saves  memory  because  it  yields  itemsone  by  one  using  the  iterator  protocol  instead  of  building  a  whole  list  just  to  feedanother constructor","prefix":"lso start from alistcomp,  but  ","suffix":".Genexps  use  the  same  syntax"}]}]}
>```
>%%
>*%%PREFIX%%lso start from alistcomp,  but%%HIGHLIGHT%% ==a  genexp  (generator  expression)  saves  memory  because  it  yields  itemsone  by  one  using  the  iterator  protocol  instead  of  building  a  whole  list  just  to  feedanother constructor== %%POSTFIX%%.Genexps  use  the  same  syntax*
>%%LINK%%[[#^qrsbdyodldm|show annotation]]
>%%COMMENT%%
>genexp are generally better because it yields to give 1 item at a time, while list comprehension feeds the whole list and all elements into at once
>
>genexp are preformed the same as list comp, but with ()
>%%TAGS%%
>
^qrsbdyodldm


>%%
>```annotation-json
>{"created":"2025-05-04T22:18:14.324Z","text":"good example of how genexp can be used, and easily scaled to large list making","updated":"2025-05-04T22:18:14.324Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":133692,"end":134158},{"type":"TextQuoteSelector","exact":"Example 2-6 uses a genexp with a Cartesian product to print out a roster of T-shirtsof two colors in three sizes. In contrast with Example 2-4, here the six-item list of T-shirts is never built in memory: the generator expression feeds the for loop produc‐ing one item at a time. If the two lists used in the Cartesian product had a thousanditems each, using a generator expression would save the cost of building a list with amillion items just to feed the for loop","prefix":"s and Generator Expressions | 29","suffix":".Example 2-6. Cartesian product "}]}]}
>```
>%%
>*%%PREFIX%%s and Generator Expressions | 29%%HIGHLIGHT%% ==Example 2-6 uses a genexp with a Cartesian product to print out a roster of T-shirtsof two colors in three sizes. In contrast with Example 2-4, here the six-item list of T-shirts is never built in memory: the generator expression feeds the for loop produc‐ing one item at a time. If the two lists used in the Cartesian product had a thousanditems each, using a generator expression would save the cost of building a list with amillion items just to feed the for loop== %%POSTFIX%%.Example 2-6. Cartesian product*
>%%LINK%%[[#^ms6gpcjlbz|show annotation]]
>%%COMMENT%%
>good example of how genexp can be used, and easily scaled to large list making
>%%TAGS%%
>
^ms6gpcjlbz


>%%
>```annotation-json
>{"created":"2025-05-04T22:20:12.266Z","text":"tuples are immutable lists AND are records with no field names (ie you can say elem1 is this and elem2 is that, and be explicit and not have someone change it)","updated":"2025-05-04T22:20:12.266Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":134988,"end":135096},{"type":"TextQuoteSelector","exact":"Tuples  do  double  duty:  they  can  be  used  as  immutable  lists  andalso as records with no field names","prefix":"t that isshort  selling  them.  ","suffix":". This use is sometimes overlook"}]}]}
>```
>%%
>*%%PREFIX%%t that isshort  selling  them.%%HIGHLIGHT%% ==Tuples  do  double  duty:  they  can  be  used  as  immutable  lists  andalso as records with no field names== %%POSTFIX%%. This use is sometimes overlook*
>%%LINK%%[[#^2cqbsr0yp8o|show annotation]]
>%%COMMENT%%
>tuples are immutable lists AND are records with no field names (ie you can say elem1 is this and elem2 is that, and be explicit and not have someone change it)
>%%TAGS%%
>
^2cqbsr0yp8o


>%%
>```annotation-json
>{"created":"2025-05-04T22:22:53.813Z","text":"ie mutable elements cannot be hashed, and so it cannot be a key to a dict","updated":"2025-05-04T22:22:53.813Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":139599,"end":139658},{"type":"TextQuoteSelector","exact":"Tuples  with  mutable  items  can  be  a  source  of  bugs.","prefix":"se>>> b(10, 'alpha', [1, 2, 99])","suffix":"  As  we’ll  see  in  “What  Is "}]}]}
>```
>%%
>*%%PREFIX%%se>>> b(10, 'alpha', [1, 2, 99])%%HIGHLIGHT%% ==Tuples  with  mutable  items  can  be  a  source  of  bugs.== %%POSTFIX%%As  we’ll  see  in  “What  Is*
>%%LINK%%[[#^vqsot8m0il|show annotation]]
>%%COMMENT%%
>ie mutable elements cannot be hashed, and so it cannot be a key to a dict
>%%TAGS%%
>
^vqsot8m0il


>%%
>```annotation-json
>{"created":"2025-05-04T22:24:45.980Z","text":"tuples are generally more efficient than lists in python\n","updated":"2025-05-04T22:24:45.980Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":140622,"end":141703},{"type":"TextQuoteSelector","exact":"To  evaluate  a  tuple  literal,  the  Python  compiler  generates  bytecode  for  a  tupleconstant  in  one  operation;  but  for  a  list  literal,  the  generated  bytecode  pusheseach element as a separate constant to the data stack, and then builds the list.• Given  a  tuple  t,  tuple(t)  simply  returns  a  reference  to  the  same  t.  There’s  noneed  to  copy.  In  contrast,  given  a  list  l,  the  list(l)  constructor  must  create  anew copy of l.• Because of its fixed length, a tuple instance is allocated the exact memory spaceit needs. Instances of list, on the other hand, are allocated with room to spare,to amortize the cost of future appends.• The  references  to  the  items  in  a  tuple  are  stored  in  an  array  in  the  tuple  struct,while  a  list  holds  a  pointer  to  an  array  of  references  stored  elsewhere.  The  indi‐rection is necessary because when a list grows beyond the space currently alloca‐ted,  Python  needs  to  reallocate  the  array  of  references  to  make  room.  The  extraindirection makes CPU caches less effective.","prefix":"To summarize, Hettinger wrote:• ","suffix":"Comparing Tuple and List Methods"}]}]}
>```
>%%
>*%%PREFIX%%To summarize, Hettinger wrote:•%%HIGHLIGHT%% ==To  evaluate  a  tuple  literal,  the  Python  compiler  generates  bytecode  for  a  tupleconstant  in  one  operation;  but  for  a  list  literal,  the  generated  bytecode  pusheseach element as a separate constant to the data stack, and then builds the list.• Given  a  tuple  t,  tuple(t)  simply  returns  a  reference  to  the  same  t.  There’s  noneed  to  copy.  In  contrast,  given  a  list  l,  the  list(l)  constructor  must  create  anew copy of l.• Because of its fixed length, a tuple instance is allocated the exact memory spaceit needs. Instances of list, on the other hand, are allocated with room to spare,to amortize the cost of future appends.• The  references  to  the  items  in  a  tuple  are  stored  in  an  array  in  the  tuple  struct,while  a  list  holds  a  pointer  to  an  array  of  references  stored  elsewhere.  The  indi‐rection is necessary because when a list grows beyond the space currently alloca‐ted,  Python  needs  to  reallocate  the  array  of  references  to  make  room.  The  extraindirection makes CPU caches less effective.== %%POSTFIX%%Comparing Tuple and List Methods*
>%%LINK%%[[#^x07qe90o8e|show annotation]]
>%%COMMENT%%
>tuples are generally more efficient than lists in python
>
>%%TAGS%%
>
^x07qe90o8e


>%%
>```annotation-json
>{"created":"2025-05-04T22:27:31.790Z","updated":"2025-05-04T22:27:31.790Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":144232,"end":144297},{"type":"TextQuoteSelector","exact":"The  most  visible  form  of  unpacking  is  parallel  assignment","prefix":"o Grab Excess Items” on page 36.","suffix":";  that  is,  assigning  itemsfr"}]}]}
>```
>%%
>*%%PREFIX%%o Grab Excess Items” on page 36.%%HIGHLIGHT%% ==The  most  visible  form  of  unpacking  is  parallel  assignment== %%POSTFIX%%;  that  is,  assigning  itemsfr*
>%%LINK%%[[#^o4rmgiuxy8|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^o4rmgiuxy8


>%%
>```annotation-json
>{"created":"2025-05-04T22:27:50.663Z","text":"\\* can be used to unpack multiple values and put that into a function directly\nt = (20, 8)\ndivmod(*t) == divmod(20,8)","updated":"2025-05-04T22:27:50.663Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":144919,"end":145076},{"type":"TextQuoteSelector","exact":"The  preceding  code  shows  another  use  of  unpacking:  allowing  functions  to  returnmultiple  values  in  a  way  that  is  convenient  to  the  caller","prefix":"*t)>>> quotient, remainder(2, 4)","suffix":".  As  another  example,  theos."}]}]}
>```
>%%
>*%%PREFIX%%*t)>>> quotient, remainder(2, 4)%%HIGHLIGHT%% ==The  preceding  code  shows  another  use  of  unpacking:  allowing  functions  to  returnmultiple  values  in  a  way  that  is  convenient  to  the  caller== %%POSTFIX%%.  As  another  example,  theos.*
>%%LINK%%[[#^1009ormxn3n|show annotation]]
>%%COMMENT%%
>\* can be used to unpack multiple values and put that into a function directly
>t = (20, 8)
>divmod(*t) == divmod(20,8)
>%%TAGS%%
>
^1009ormxn3n


>%%
>```annotation-json
>{"created":"2025-05-04T22:29:01.358Z","text":"\\* can be used to grab all remaining, unassigned values and put it in a list (if they exist). ","updated":"2025-05-04T22:29:01.358Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":145393,"end":145421},{"type":"TextQuoteSelector","exact":"Using * to Grab Excess Items","prefix":" syntax, aswe’ll see right away.","suffix":"Defining  function  parameters  "}]}]}
>```
>%%
>*%%PREFIX%%syntax, aswe’ll see right away.%%HIGHLIGHT%% ==Using * to Grab Excess Items== %%POSTFIX%%Defining  function  parameters*
>%%LINK%%[[#^llfvs91cknj|show annotation]]
>%%COMMENT%%
>\* can be used to grab all remaining, unassigned values and put it in a list (if they exist). 
>%%TAGS%%
>
^llfvs91cknj


>%%
>```annotation-json
>{"created":"2025-05-04T22:33:31.416Z","text":"match/case can store values within the cases' themselves\n\nNote that match/case was introduced in Python3.10","updated":"2025-05-04T22:33:31.416Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":150129,"end":150178},{"type":"TextQuoteSelector","exact":"Example 2-9. Method from an imaginary Robot class","prefix":"ke this to handle such messages:","suffix":"    def handle_command(self, mes"}]}]}
>```
>%%
>*%%PREFIX%%ke this to handle such messages:%%HIGHLIGHT%% ==Example 2-9. Method from an imaginary Robot class== %%POSTFIX%%def handle_command(self, mes*
>%%LINK%%[[#^87uqcetaj8q|show annotation]]
>%%COMMENT%%
>match/case can store values within the cases' themselves
>
>Note that match/case was introduced in Python3.10
>%%TAGS%%
>
^87uqcetaj8q


>%%
>```annotation-json
>{"created":"2025-05-04T22:34:29.639Z","text":"destructuring - you can match formats instead of switching on specific cases of the the arguments provided\n\nmakes match/case stronger than switch/case","updated":"2025-05-04T22:34:29.639Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":151992,"end":152082},{"type":"TextQuoteSelector","exact":"One key improvement of match over switch isdestructuring—a more advanced form of unpacking","prefix":"ut that’s only half the story.4 ","suffix":". Destructuring is a new word in"}]}]}
>```
>%%
>*%%PREFIX%%ut that’s only half the story.4%%HIGHLIGHT%% ==One key improvement of match over switch isdestructuring—a more advanced form of unpacking== %%POSTFIX%%. Destructuring is a new word in*
>%%LINK%%[[#^b6hou2jnxg6|show annotation]]
>%%COMMENT%%
>destructuring - you can match formats instead of switching on specific cases of the the arguments provided
>
>makes match/case stronger than switch/case
>%%TAGS%%
>
^b6hou2jnxg6


>%%
>```annotation-json
>{"created":"2025-05-04T22:38:11.787Z","text":"case [str(name), _, _, (float(lat), float(lon))]:\n\nwhere str() and float() are actually typechecking the values from unpacking!","updated":"2025-05-04T22:38:11.787Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":155942,"end":156685},{"type":"TextQuoteSelector","exact":"The  expressions  str(name)  and  float(lat)  look  like  constructorcalls,  which  we’d  use  to  convert  name  and  lat  to  str  and  float.But in the context of a pattern, that syntax performs a runtime typecheck:  the  preceding  pattern  will  match  a  four-item  sequence  inwhich  item  0  must  be  a  str,  and  item  3  must  be  a  pair  of  floats.Additionally, the str in item 0 will be bound to the name variable,and the floats in item 3 will be bound to lat and lon, respectively.So,  although  str(name)  borrows  the  syntax  of  a  constructor  call,the  semantics  are  completely  different  in  the  context  of  a  pattern.Using arbitrary classes in patterns is covered in “Pattern MatchingClass Instances” on page 192","prefix":"_, _, (float(lat), float(lon))]:","suffix":".On the other hand, if we want t"}]}]}
>```
>%%
>*%%PREFIX%%_, _, (float(lat), float(lon))]:%%HIGHLIGHT%% ==The  expressions  str(name)  and  float(lat)  look  like  constructorcalls,  which  we’d  use  to  convert  name  and  lat  to  str  and  float.But in the context of a pattern, that syntax performs a runtime typecheck:  the  preceding  pattern  will  match  a  four-item  sequence  inwhich  item  0  must  be  a  str,  and  item  3  must  be  a  pair  of  floats.Additionally, the str in item 0 will be bound to the name variable,and the floats in item 3 will be bound to lat and lon, respectively.So,  although  str(name)  borrows  the  syntax  of  a  constructor  call,the  semantics  are  completely  different  in  the  context  of  a  pattern.Using arbitrary classes in patterns is covered in “Pattern MatchingClass Instances” on page 192== %%POSTFIX%%.On the other hand, if we want t*
>%%LINK%%[[#^czv2mhrjfio|show annotation]]
>%%COMMENT%%
>case [str(name), _, _, (float(lat), float(lon))]:
>
>where str() and float() are actually typechecking the values from unpacking!
>%%TAGS%%
>
^czv2mhrjfio


>%%
>```annotation-json
>{"created":"2025-05-04T22:51:34.129Z","updated":"2025-05-04T22:51:34.129Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":162228,"end":162358},{"type":"TextQuoteSelector","exact":"Without a catch-all, the whole match statement does nothing when a subject does notmatch any case—and this can be a silent failure","prefix":"formed, and I raise SyntaxError.","suffix":".Norvig  deliberately  avoided  "}]}]}
>```
>%%
>*%%PREFIX%%formed, and I raise SyntaxError.%%HIGHLIGHT%% ==Without a catch-all, the whole match statement does nothing when a subject does notmatch any case—and this can be a silent failure== %%POSTFIX%%.Norvig  deliberately  avoided*
>%%LINK%%[[#^sgq7g91wq2l|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^sgq7g91wq2l


>%%
>```annotation-json
>{"created":"2025-05-04T22:55:49.755Z","text":"how slicing is performed as a special method. Generally is it already implemented for you when you implement \\__getitem\\__","updated":"2025-05-04T22:55:49.755Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":168824,"end":168934},{"type":"TextQuoteSelector","exact":"to  evaluate  the  expression  seq[start:stop:step],  Pythoncalls  seq.__getitem__(slice(start,  stop,  step))","prefix":"ic‐ing  Works”  on  page  404,  ","suffix":".  Even  if  you  are  not  impl"}]}]}
>```
>%%
>*%%PREFIX%%ic‐ing  Works”  on  page  404,%%HIGHLIGHT%% ==to  evaluate  the  expression  seq[start:stop:step],  Pythoncalls  seq.__getitem__(slice(start,  stop,  step))== %%POSTFIX%%.  Even  if  you  are  not  impl*
>%%LINK%%[[#^rpzmwvigwed|show annotation]]
>%%COMMENT%%
>how slicing is performed as a special method. Generally is it already implemented for you when you implement \__getitem\__
>%%TAGS%%
>
^rpzmwvigwed


>%%
>```annotation-json
>{"created":"2025-05-04T23:11:26.679Z","updated":"2025-05-04T23:11:26.679Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":173295,"end":173417},{"type":"TextQuoteSelector","exact":"When the target of the assignment is a slice, the righthand side must be an itera‐ble object, even if it has just one item","prefix":"] = [100]>>> l[0, 1, 100, 22, 9]","suffix":".Every coder knows that concaten"}]}]}
>```
>%%
>*%%PREFIX%%] = [100]>>> l[0, 1, 100, 22, 9]%%HIGHLIGHT%% ==When the target of the assignment is a slice, the righthand side must be an itera‐ble object, even if it has just one item== %%POSTFIX%%.Every coder knows that concaten*
>%%LINK%%[[#^r1jidr74vo|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^r1jidr74vo


>%%
>```annotation-json
>{"created":"2025-05-04T23:12:20.470Z","text":"you may need to copy the values inside of [a]*n if you want each instance to be unique (given that a is a reference variable)\n\nessentailly it is doing\nfor i in range(n):\n... list.append(a)","updated":"2025-05-04T23:12:20.470Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":174282,"end":174602},{"type":"TextQuoteSelector","exact":"Beware  of  expressions  like  a * n  when  a  is  a  sequence  containingmutable  items,  because  the  result  may  surprise  you.  For  example,trying  to  initialize  a  list  of  lists  as  my_list = [[]] * 3  will  resultin a list with three references to the same inner list, which is proba‐bly not what you want.","prefix":"and never change their operands.","suffix":"The next section covers the pitf"}]}]}
>```
>%%
>*%%PREFIX%%and never change their operands.%%HIGHLIGHT%% ==Beware  of  expressions  like  a * n  when  a  is  a  sequence  containingmutable  items,  because  the  result  may  surprise  you.  For  example,trying  to  initialize  a  list  of  lists  as  my_list = [[]] * 3  will  resultin a list with three references to the same inner list, which is proba‐bly not what you want.== %%POSTFIX%%The next section covers the pitf*
>%%LINK%%[[#^wo02117gfj|show annotation]]
>%%COMMENT%%
>you may need to copy the values inside of [a]*n if you want each instance to be unique (given that a is a reference variable)
>
>essentailly it is doing
>for i in range(n):
>... list.append(a)
>%%TAGS%%
>
^wo02117gfj


>%%
>```annotation-json
>{"created":"2025-05-04T23:17:07.112Z","text":"good example of somewhat unexpected behaviour from the above code that is correct `board = [['_'] * 3 for i in range(3)]`","updated":"2025-05-04T23:17:07.112Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":175441,"end":175511},{"type":"TextQuoteSelector","exact":"Example 2-15. A list with three references to the same list is useless","prefix":"t is doing it like Example 2-15.","suffix":">>> weird_board = [['_'] * 3] * "}]}]}
>```
>%%
>*%%PREFIX%%t is doing it like Example 2-15.%%HIGHLIGHT%% ==Example 2-15. A list with three references to the same list is useless== %%POSTFIX%%>>> weird_board = [['_'] * 3] **
>%%LINK%%[[#^no9ealc5qbp|show annotation]]
>%%COMMENT%%
>good example of somewhat unexpected behaviour from the above code that is correct `board = [['_'] * 3 for i in range(3)]`
>%%TAGS%%
>
^no9ealc5qbp


>%%
>```annotation-json
>{"created":"2025-05-04T23:19:11.368Z","text":"\\__iadd\\__ and other special methods like it are able to keep the same reference for a after performing the operation, otherwise the default operation will take place and will need to explicilty make a new object","updated":"2025-05-04T23:19:11.368Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":177583,"end":178126},{"type":"TextQuoteSelector","exact":"If a implements __iadd__, that will be called. In the case of mutable sequences (e.g.,list, bytearray, array.array), a will be changed in place (i.e., the effect will be sim‐ilar to a.extend(b)). However, when a does not implement __iadd__, the expressiona += b  has  the  same  effect  as  a = a + b:  the  expression  a + b  is  evaluated  first,producing  a  new  object,  which  is  then  bound  to  a.  In  other  words,  the  identity  ofthe  object  bound  to  a  may  or  may  not  change,  depending  on  the  availability  of__iadd__","prefix":"his simple expression:>>> a += b","suffix":".In general, for mutable sequenc"}]}]}
>```
>%%
>*%%PREFIX%%his simple expression:>>> a += b%%HIGHLIGHT%% ==If a implements __iadd__, that will be called. In the case of mutable sequences (e.g.,list, bytearray, array.array), a will be changed in place (i.e., the effect will be sim‐ilar to a.extend(b)). However, when a does not implement __iadd__, the expressiona += b  has  the  same  effect  as  a = a + b:  the  expression  a + b  is  evaluated  first,producing  a  new  object,  which  is  then  bound  to  a.  In  other  words,  the  identity  ofthe  object  bound  to  a  may  or  may  not  change,  depending  on  the  availability  of__iadd__== %%POSTFIX%%.In general, for mutable sequenc*
>%%LINK%%[[#^y4qadyv7w8f|show annotation]]
>%%COMMENT%%
>\__iadd\__ and other special methods like it are able to keep the same reference for a after performing the operation, otherwise the default operation will take place and will need to explicilty make a new object
>%%TAGS%%
>
^y4qadyv7w8f


>%%
>```annotation-json
>{"created":"2025-05-05T04:24:18.827Z","text":"very weird behaviour, has an error but proceeds to do the assignment anyways. \n\nThis is because it is OK to do t[2]+=[50,60], and it proceeds as normal, however the interpreter realizes the original type of t is a tupe and there is the error","updated":"2025-05-05T04:24:18.827Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":180314,"end":180463},{"type":"TextQuoteSelector","exact":"When I saw this, I was pretty sure the answer was B, but it’s actually D, “Both A andB”! Example 2-17 is the actual output from a Python 3.9 console.","prefix":"ment.C. Neither.D. Both A and B.","suffix":"1054 | Chapter 2: An Array of Se"}]}]}
>```
>%%
>*%%PREFIX%%ment.C. Neither.D. Both A and B.%%HIGHLIGHT%% ==When I saw this, I was pretty sure the answer was B, but it’s actually D, “Both A andB”! Example 2-17 is the actual output from a Python 3.9 console.== %%POSTFIX%%1054 | Chapter 2: An Array of Se*
>%%LINK%%[[#^0f19ptky39t4|show annotation]]
>%%COMMENT%%
>very weird behaviour, has an error but proceeds to do the assignment anyways. 
>
>This is because it is OK to do t[2]+=[50,60], and it proceeds as normal, however the interpreter realizes the original type of t is a tupe and there is the error
>%%TAGS%%
>
^0f19ptky39t4


>%%
>```annotation-json
>{"created":"2025-05-05T04:36:24.863Z","text":"Online Python Tutor goes line by line and shows what python is doing ","updated":"2025-05-05T04:36:24.863Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":180786,"end":180882},{"type":"TextQuoteSelector","exact":"Online  Python  Tutor  is  an  awesome  online  tool  to  visualize  how  Python  works  indetai","prefix":"ent>>> t(1, 2, [30, 40, 50, 60])","suffix":"l. Figure 2-5 is a composite of "}]}]}
>```
>%%
>*%%PREFIX%%ent>>> t(1, 2, [30, 40, 50, 60])%%HIGHLIGHT%% ==Online  Python  Tutor  is  an  awesome  online  tool  to  visualize  how  Python  works  indetai== %%POSTFIX%%l. Figure 2-5 is a composite of*
>%%LINK%%[[#^7pjbbvlwqtd|show annotation]]
>%%COMMENT%%
>Online Python Tutor goes line by line and shows what python is doing 
>%%TAGS%%
>
^7pjbbvlwqtd


>%%
>```annotation-json
>{"created":"2025-05-05T04:37:54.006Z","text":"functions or methods that change objects inplace should return None","updated":"2025-05-05T04:37:54.006Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":182860,"end":183063},{"type":"TextQuoteSelector","exact":"This isan important Python API convention: functions or methods that change an object inplace should return None to make it clear to the caller that the receiver was changed,and no new object was created","prefix":"and does not create a new list. ","suffix":". Similar behavior can be seen, "}]}]}
>```
>%%
>*%%PREFIX%%and does not create a new list.%%HIGHLIGHT%% ==This isan important Python API convention: functions or methods that change an object inplace should return None to make it clear to the caller that the receiver was changed,and no new object was created== %%POSTFIX%%. Similar behavior can be seen,*
>%%LINK%%[[#^61162chxvla|show annotation]]
>%%COMMENT%%
>functions or methods that change objects inplace should return None
>%%TAGS%%
>
^61162chxvla


>%%
>```annotation-json
>{"created":"2025-05-05T06:00:36.160Z","text":"sorting requires 2 arguments\n* reverse - bool to reverse or not, defaults false\n* key - comparision type, can be len, str.lower, etc., defaults to  the identity function that compares items","updated":"2025-05-05T06:00:36.160Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":184034,"end":184101},{"type":"TextQuoteSelector","exact":"Both list.sort and sorted take two optional, keyword-only arguments","prefix":"ays returns anewly created list.","suffix":":reverseIf True, the items are r"}]}]}
>```
>%%
>*%%PREFIX%%ays returns anewly created list.%%HIGHLIGHT%% ==Both list.sort and sorted take two optional, keyword-only arguments== %%POSTFIX%%:reverseIf True, the items are r*
>%%LINK%%[[#^a8tswf2dwvd|show annotation]]
>%%COMMENT%%
>sorting requires 2 arguments
>* reverse - bool to reverse or not, defaults false
>* key - comparision type, can be len, str.lower, etc., defaults to  the identity function that compares items
>%%TAGS%%
>
^a8tswf2dwvd


>%%
>```annotation-json
>{"created":"2025-05-05T17:01:13.754Z","text":"array.array: lists for numerical values only. As close to a C array as we have. ","updated":"2025-05-05T17:01:13.754Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":188680,"end":188818},{"type":"TextQuoteSelector","exact":"If  a  list  only  contains  numbers,  an  array.array  is  a  more  efficient  replacement.Arrays support all mutable sequence operations","prefix":"ses, starting with arrays.Arrays","suffix":" (including .pop, .insert,and .e"}]}]}
>```
>%%
>*%%PREFIX%%ses, starting with arrays.Arrays%%HIGHLIGHT%% ==If  a  list  only  contains  numbers,  an  array.array  is  a  more  efficient  replacement.Arrays support all mutable sequence operations== %%POSTFIX%%(including .pop, .insert,and .e*
>%%LINK%%[[#^7b2yt7h9ch|show annotation]]
>%%COMMENT%%
>array.array: lists for numerical values only. As close to a C array as we have. 
>%%TAGS%%
>
^7b2yt7h9ch


>%%
>```annotation-json
>{"created":"2025-05-05T17:02:27.510Z","text":"using array.array, you must declare what type of numerical value you put inside of it, which can save a lot of data at scale","updated":"2025-05-05T17:02:27.510Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":189487,"end":189741},{"type":"TextQuoteSelector","exact":"If  you  create  anarray('b'), then each item will be stored in a single byte and interpreted as an inte‐ger. For large sequences of numbers, this saves a lot of memory. And Python will notlet you put any number that does not match the type for the array","prefix":" ranging  from  –128  to  127.  ","suffix":".Example  2-19  shows  creating,"}]}]}
>```
>%%
>*%%PREFIX%%ranging  from  –128  to  127.%%HIGHLIGHT%% ==If  you  create  anarray('b'), then each item will be stored in a single byte and interpreted as an inte‐ger. For large sequences of numbers, this saves a lot of memory. And Python will notlet you put any number that does not match the type for the array== %%POSTFIX%%.Example  2-19  shows  creating,*
>%%LINK%%[[#^luy8lk03im|show annotation]]
>%%COMMENT%%
>using array.array, you must declare what type of numerical value you put inside of it, which can save a lot of data at scale
>%%TAGS%%
>
^luy8lk03im


>%%
>```annotation-json
>{"created":"2025-05-05T17:04:42.129Z","text":"saving these arrays are much faster to read/write to and compresses way more than to text files","updated":"2025-05-05T17:04:42.129Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":190719,"end":191490},{"type":"TextQuoteSelector","exact":"As  you  can  see,  array.tofile  and  array.fromfile  are  easy  to  use.  If  you  try  theexample, you’ll notice they are also very fast. A quick experiment shows that it takesabout  0.1  seconds  for  array.fromfile  to  load  10  million  double-precision  floatsfrom  a  binary  file  created  with  array.tofile.  That  is  nearly  60  times  faster  thanreading  the  numbers  from  a  text  file,  which  also  involves  parsing  each  line  with  thefloat built-in. Saving with array.tofile is about seven times faster than writing onefloat per line in a text file. In addition, the size of the binary file with 10 million dou‐bles  is  80,000,000  bytes  (8  bytes  per  double,  zero  overhead),  while  the  text  file  has181,515,739 bytes for the same data","prefix":"he contents of the arrays match.","suffix":".60 | Chapter 2: An Array of Seq"}]}]}
>```
>%%
>*%%PREFIX%%he contents of the arrays match.%%HIGHLIGHT%% ==As  you  can  see,  array.tofile  and  array.fromfile  are  easy  to  use.  If  you  try  theexample, you’ll notice they are also very fast. A quick experiment shows that it takesabout  0.1  seconds  for  array.fromfile  to  load  10  million  double-precision  floatsfrom  a  binary  file  created  with  array.tofile.  That  is  nearly  60  times  faster  thanreading  the  numbers  from  a  text  file,  which  also  involves  parsing  each  line  with  thefloat built-in. Saving with array.tofile is about seven times faster than writing onefloat per line in a text file. In addition, the size of the binary file with 10 million dou‐bles  is  80,000,000  bytes  (8  bytes  per  double,  zero  overhead),  while  the  text  file  has181,515,739 bytes for the same data== %%POSTFIX%%.60 | Chapter 2: An Array of Seq*
>%%LINK%%[[#^d6t2bzk47bs|show annotation]]
>%%COMMENT%%
>saving these arrays are much faster to read/write to and compresses way more than to text files
>%%TAGS%%
>
^d6t2bzk47bs


>%%
>```annotation-json
>{"created":"2025-05-05T17:07:13.676Z","text":"memmoryview - an builtin python array that allows you to share memory between data structures without first copying! Super imporant for large datasets\n\nIn the example below, we can declare an array octets and then send that value to memoryview, augment the values inside, and then verify that octets was changed. (They use the same memory values!)","updated":"2025-05-05T17:07:13.676Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":194743,"end":195047},{"type":"TextQuoteSelector","exact":"A  memoryview  is  essentially  a  generalized  NumPy  array  structure  in  Python  itself(without the math). It allows you to share memory between data-structures (things likePIL  images,  SQLite  databases,  NumPy  arrays,  etc.)  without  first  copying.  This  is  veryimportant for large data sets.","prefix":" memoryview be used?” like this:","suffix":"Using  notation  similar  to  th"}]}]}
>```
>%%
>*%%PREFIX%%memoryview be used?” like this:%%HIGHLIGHT%% ==A  memoryview  is  essentially  a  generalized  NumPy  array  structure  in  Python  itself(without the math). It allows you to share memory between data-structures (things likePIL  images,  SQLite  databases,  NumPy  arrays,  etc.)  without  first  copying.  This  is  veryimportant for large data sets.== %%POSTFIX%%Using  notation  similar  to  th*
>%%LINK%%[[#^b8yarwhpxna|show annotation]]
>%%COMMENT%%
>memmoryview - an builtin python array that allows you to share memory between data structures without first copying! Super imporant for large datasets
>
>In the example below, we can declare an array octets and then send that value to memoryview, augment the values inside, and then verify that octets was changed. (They use the same memory values!)
>%%TAGS%%
>
^b8yarwhpxna


>%%
>```annotation-json
>{"created":"2025-05-05T17:08:39.147Z","text":"memoryview.cast allows you to change how the values are partiioned\nmemoryview.cast( <# of partitions>, <#size of each partition>)","updated":"2025-05-05T17:08:39.147Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":195098,"end":195320},{"type":"TextQuoteSelector","exact":"the  memoryview.cast  method  lets  youchange  the  way  multiple  bytes  are  read  or  written  as  units  without  moving  bitsaround. memoryview.cast returns yet another memoryview object, always sharing thesame memory","prefix":"milar  to  the  array  module,  ","suffix":".Example  2-20  shows  how  to  "}]}]}
>```
>%%
>*%%PREFIX%%milar  to  the  array  module,%%HIGHLIGHT%% ==the  memoryview.cast  method  lets  youchange  the  way  multiple  bytes  are  read  or  written  as  units  without  moving  bitsaround. memoryview.cast returns yet another memoryview object, always sharing thesame memory== %%POSTFIX%%.Example  2-20  shows  how  to*
>%%LINK%%[[#^o6shh7nqzu|show annotation]]
>%%COMMENT%%
>memoryview.cast allows you to change how the values are partiioned
>memoryview.cast( <# of partitions>, <#size of each partition>)
>%%TAGS%%
>
^o6shh7nqzu


>%%
>```annotation-json
>{"created":"2025-05-05T17:14:11.769Z","text":"some example code of using numpy for augmenting arrays","updated":"2025-05-05T17:14:11.769Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":198690,"end":198761},{"type":"TextQuoteSelector","exact":"Example 2-22. Basic operations with rows and columns in a numpy.ndarray","prefix":"Chapter 2: An Array of Sequences","suffix":">>> import numpy as np >>> a = n"}]}]}
>```
>%%
>*%%PREFIX%%Chapter 2: An Array of Sequences%%HIGHLIGHT%% ==Example 2-22. Basic operations with rows and columns in a numpy.ndarray== %%POSTFIX%%>>> import numpy as np >>> a = n*
>%%LINK%%[[#^q68xbv35y9|show annotation]]
>%%COMMENT%%
>some example code of using numpy for augmenting arrays
>%%TAGS%%
>
^q68xbv35y9


>%%
>```annotation-json
>{"created":"2025-05-05T17:16:15.323Z","text":"THESE PROGRAMS ARE AS EFFICIENT AS THEY CAN BE, because they don't rely on the GIL and and be ran on all CPU cores","updated":"2025-05-05T17:16:15.323Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":201442,"end":201613},{"type":"TextQuoteSelector","exact":" Most  NumPy  and  SciPy  functions  are  implementedin  C  or  C++,  and  can  leverage  all  CPU  cores  because  they  release  Python’s  GIL(Global  Interpreter  Lock)","prefix":"ed  Machine  Learning  toolset. ","suffix":".  The  Dask  project  supports "}]}]}
>```
>%%
>*%%PREFIX%%ed  Machine  Learning  toolset.%%HIGHLIGHT%% ==Most  NumPy  and  SciPy  functions  are  implementedin  C  or  C++,  and  can  leverage  all  CPU  cores  because  they  release  Python’s  GIL(Global  Interpreter  Lock)== %%POSTFIX%%.  The  Dask  project  supports*
>%%LINK%%[[#^s1glc267kpi|show annotation]]
>%%COMMENT%%
>THESE PROGRAMS ARE AS EFFICIENT AS THEY CAN BE, because they don't rely on the GIL and and be ran on all CPU cores
>%%TAGS%%
>
^s1glc267kpi


>%%
>```annotation-json
>{"created":"2025-05-05T17:24:35.951Z","text":"collections.deque is a double ended thread safe queue. \n\nIt allows you to specify a maxlen for the max # of elements you can have in it, and will automatically remove the values.\n\n* rotate moves values from left to right if n>0, right to left if n<0 \n* appendleft appends values to the left\n* appendleft appends values to the left\n* extend adds values to the right\n* extendLeft adds values to the left side, going sequentially down the list, so the extended result is reversed\n","updated":"2025-05-05T17:24:35.951Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":202405,"end":202803},{"type":"TextQuoteSelector","exact":"The  class  collections.deque  is  a  thread-safe  double-ended  queue  designed  for  fastinserting and removing from both ends. It is also the way to go if you need to keep alist of “last seen items” or something of that nature, because a deque can be bounded—i.e., created with a fixed maximum length. If a bounded deque is full, when you adda new item, it discards an item from the opposite end","prefix":"e list must be shifted inmemory.","suffix":". Example 2-23 shows some typ‐ic"}]}]}
>```
>%%
>*%%PREFIX%%e list must be shifted inmemory.%%HIGHLIGHT%% ==The  class  collections.deque  is  a  thread-safe  double-ended  queue  designed  for  fastinserting and removing from both ends. It is also the way to go if you need to keep alist of “last seen items” or something of that nature, because a deque can be bounded—i.e., created with a fixed maximum length. If a bounded deque is full, when you adda new item, it discards an item from the opposite end== %%POSTFIX%%. Example 2-23 shows some typ‐ic*
>%%LINK%%[[#^0ztkxs9olpyq|show annotation]]
>%%COMMENT%%
>collections.deque is a double ended thread safe queue. 
>
>It allows you to specify a maxlen for the max # of elements you can have in it, and will automatically remove the values.
>
>* rotate moves values from left to right if n>0, right to left if n<0 
>* appendleft appends values to the left
>* appendleft appends values to the left
>* extend adds values to the right
>* extendLeft adds values to the left side, going sequentially down the list, so the extended result is reversed
>
>%%TAGS%%
>
^0ztkxs9olpyq


>%%
>```annotation-json
>{"created":"2025-05-05T17:27:26.981Z","updated":"2025-05-05T17:27:26.981Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":204399,"end":204568},{"type":"TextQuoteSelector","exact":" But  there  is  a  hidden  cost:  removingitems  from  the  middle  of  a  deque  is  not  as  fast.  It  is  really  optimized  for  appendingand popping from the ends","prefix":"n,  like  popleft  and  rotate. ","suffix":".The  append  and  popleft  oper"}]}]}
>```
>%%
>*%%PREFIX%%n,  like  popleft  and  rotate.%%HIGHLIGHT%% ==But  there  is  a  hidden  cost:  removingitems  from  the  middle  of  a  deque  is  not  as  fast.  It  is  really  optimized  for  appendingand popping from the ends== %%POSTFIX%%.The  append  and  popleft  oper*
>%%LINK%%[[#^4o7jslk00ha|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^4o7jslk00ha


>%%
>```annotation-json
>{"created":"2025-05-05T17:28:54.257Z","text":"queue will wait there is space to push a new item if there is no space inside of it currently, will not discard items","updated":"2025-05-05T17:28:54.257Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":206860,"end":207128},{"type":"TextQuoteSelector","exact":" However,  they  don’t  discarditems to make room as deque does. Instead, when the queue is full, the insertionof a new item blocks—i.e., it waits until some other thread makes room by takingan item from the queue, which is useful to throttle the number of live thread","prefix":" than  0  to  the  constructor. ","suffix":"s.multiprocessingImplements  its"}]}]}
>```
>%%
>*%%PREFIX%%than  0  to  the  constructor.%%HIGHLIGHT%% ==However,  they  don’t  discarditems to make room as deque does. Instead, when the queue is full, the insertionof a new item blocks—i.e., it waits until some other thread makes room by takingan item from the queue, which is useful to throttle the number of live thread== %%POSTFIX%%s.multiprocessingImplements  its*
>%%LINK%%[[#^1vj6e66s50j|show annotation]]
>%%COMMENT%%
>queue will wait there is space to push a new item if there is no space inside of it currently, will not discard items
>%%TAGS%%
>
^1vj6e66s50j


>%%
>```annotation-json
>{"created":"2025-05-05T17:39:56.858Z","text":"asyncio is for queues that are aysncronous","updated":"2025-05-05T17:39:56.858Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":207395,"end":207587},{"type":"TextQuoteSelector","exact":"Provides Queue, LifoQueue, PriorityQueue, and JoinableQueue with APIsinspired by the classes in the queue and multiprocessing modules, but adaptedfor managing tasks in asynchronous programming","prefix":"ided for task management.asyncio","suffix":".heapqIn  contrast  to  the  pre"}]}]}
>```
>%%
>*%%PREFIX%%ided for task management.asyncio%%HIGHLIGHT%% ==Provides Queue, LifoQueue, PriorityQueue, and JoinableQueue with APIsinspired by the classes in the queue and multiprocessing modules, but adaptedfor managing tasks in asynchronous programming== %%POSTFIX%%.heapqIn  contrast  to  the  pre*
>%%LINK%%[[#^6gygi0axshq|show annotation]]
>%%COMMENT%%
>asyncio is for queues that are aysncronous
>%%TAGS%%
>
^6gygi0axshq


>%%
>```annotation-json
>{"created":"2025-05-05T17:40:15.328Z","text":"multiprocessing is for queues that are between processes","updated":"2025-05-05T17:40:15.328Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":207145,"end":207386},{"type":"TextQuoteSelector","exact":"Implements  its  own  unbounded  SimpleQueue  and  bounded  Queue,  very  similarto  those  in  the  queue  package,  but  designed  for  interprocess  communication.  Aspecialized multiprocessing.JoinableQueue is provided for task managemen","prefix":" of live threads.multiprocessing","suffix":"t.asyncioProvides Queue, LifoQue"}]}]}
>```
>%%
>*%%PREFIX%%of live threads.multiprocessing%%HIGHLIGHT%% ==Implements  its  own  unbounded  SimpleQueue  and  bounded  Queue,  very  similarto  those  in  the  queue  package,  but  designed  for  interprocess  communication.  Aspecialized multiprocessing.JoinableQueue is provided for task managemen== %%POSTFIX%%t.asyncioProvides Queue, LifoQue*
>%%LINK%%[[#^d9ep376o21|show annotation]]
>%%COMMENT%%
>multiprocessing is for queues that are between processes
>%%TAGS%%
>
^d9ep376o21


>%%
>```annotation-json
>{"created":"2025-05-05T17:40:46.404Z","text":"heapq turns mutable seqeueunces into a heap queue or priority queue\n","updated":"2025-05-05T17:40:46.404Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":207593,"end":207806},{"type":"TextQuoteSelector","exact":"In  contrast  to  the  previous  three  modules,  heapq  does  not  implement  a  queueclass, but provides functions like heappush and heappop that let you use a muta‐ble sequence as a heap queue or priority queue","prefix":"n asynchronous programming.heapq","suffix":".When a List Is Not the Answer |"}]}]}
>```
>%%
>*%%PREFIX%%n asynchronous programming.heapq%%HIGHLIGHT%% ==In  contrast  to  the  previous  three  modules,  heapq  does  not  implement  a  queueclass, but provides functions like heappush and heappop that let you use a muta‐ble sequence as a heap queue or priority queue== %%POSTFIX%%.When a List Is Not the Answer |*
>%%LINK%%[[#^qsmphkg310o|show annotation]]
>%%COMMENT%%
>heapq turns mutable seqeueunces into a heap queue or priority queue
>
>%%TAGS%%
>
^qsmphkg310o


>%%
>```annotation-json
>{"created":"2025-05-05T18:04:28.669Z","text":"\\** allows you to unpack mappings, where duplicate values are overwritten","updated":"2025-05-05T18:04:28.669Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":228008,"end":228072},{"type":"TextQuoteSelector","exact":"Second, ** can be used inside a dict literal—also multiple times","prefix":"'z': 3}){'x': 1, 'y': 2, 'z': 3}","suffix":":>>> {'a': 0, **{'x': 1}, 'y': 2"}]}]}
>```
>%%
>*%%PREFIX%%'z': 3}){'x': 1, 'y': 2, 'z': 3}%%HIGHLIGHT%% ==Second, ** can be used inside a dict literal—also multiple times== %%POSTFIX%%:>>> {'a': 0, **{'x': 1}, 'y': 2*
>%%LINK%%[[#^wrd435ihrh|show annotation]]
>%%COMMENT%%
>\** allows you to unpack mappings, where duplicate values are overwritten
>%%TAGS%%
>
^wrd435ihrh


>%%
>```annotation-json
>{"created":"2025-05-05T18:05:28.477Z","updated":"2025-05-05T18:05:28.477Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":228393,"end":228508},{"type":"TextQuoteSelector","exact":"Python 3.9 supports using | and |= to merge mappings. This makes sense, since theseare also the set union operators","prefix":"e readon.Merging Mappings with |","suffix":".The | operator creates a new ma"}]}]}
>```
>%%
>*%%PREFIX%%e readon.Merging Mappings with |%%HIGHLIGHT%% ==Python 3.9 supports using | and |= to merge mappings. This makes sense, since theseare also the set union operators== %%POSTFIX%%.The | operator creates a new ma*
>%%LINK%%[[#^g77iqd781fq|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^g77iqd781fq


>%%
>```annotation-json
>{"created":"2025-05-05T18:08:45.965Z","text":"mapping patterns only need partial matches","updated":"2025-05-05T18:08:45.965Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":232788,"end":232987},{"type":"TextQuoteSelector","exact":"In contrast with sequence patterns, mapping patterns succeed on partial matches. Inthe doctests, the b1 and b2 subjects include a 'title' key that does not appear in any'book' pattern, yet they match","prefix":"Chapter 3: Dictionaries and Sets","suffix":".There  is  no  need  to  use  *"}]}]}
>```
>%%
>*%%PREFIX%%Chapter 3: Dictionaries and Sets%%HIGHLIGHT%% ==In contrast with sequence patterns, mapping patterns succeed on partial matches. Inthe doctests, the b1 and b2 subjects include a 'title' key that does not appear in any'book' pattern, yet they match== %%POSTFIX%%.There  is  no  need  to  use  **
>%%LINK%%[[#^pntw1f8dzqb|show annotation]]
>%%COMMENT%%
>mapping patterns only need partial matches
>%%TAGS%%
>
^pntw1f8dzqb


>%%
>```annotation-json
>{"created":"2025-05-05T18:09:31.785Z","text":"**extra must be used at the end to get all key-values pairs that were not matched before","updated":"2025-05-05T18:09:31.785Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":233025,"end":233232},{"type":"TextQuoteSelector","exact":"  to  match  extra  key-value  pairs,  but  if  you  want  tocapture them as a dict, you can prefix one variable with **. It must be the last in thepattern, and **_ is forbidden because it would be redundant","prefix":"  is  no  need  to  use  **extra","suffix":". A simple example:>>> food = di"}]}]}
>```
>%%
>*%%PREFIX%%is  no  need  to  use  **extra%%HIGHLIGHT%% ==to  match  extra  key-value  pairs,  but  if  you  want  tocapture them as a dict, you can prefix one variable with **. It must be the last in thepattern, and **_ is forbidden because it would be redundant== %%POSTFIX%%. A simple example:>>> food = di*
>%%LINK%%[[#^18s0dh8bqkn|show annotation]]
>%%COMMENT%%
>**extra must be used at the end to get all key-values pairs that were not matched before
>%%TAGS%%
>
^18s0dh8bqkn


>%%
>```annotation-json
>{"created":"2025-05-05T18:17:55.873Z","text":"use collections.UserDict to make a custom mapping for a dictionary if you so need to make on for ti","updated":"2025-05-05T18:17:55.873Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":235424,"end":235746},{"type":"TextQuoteSelector","exact":"To implement a custom mapping, it’s easier to extend collections.UserDict, or towrap a dict by composition, instead of subclassing these ABCs. The collections.UserDict class and all concrete mapping classes in the standard library encap‐sulate the basic dict in their implementation, which in turn is built on a hash table","prefix":"t classes and abstract methods).","suffix":".Therefore,  they  all  share  t"}]}]}
>```
>%%
>*%%PREFIX%%t classes and abstract methods).%%HIGHLIGHT%% ==To implement a custom mapping, it’s easier to extend collections.UserDict, or towrap a dict by composition, instead of subclassing these ABCs. The collections.UserDict class and all concrete mapping classes in the standard library encap‐sulate the basic dict in their implementation, which in turn is built on a hash table== %%POSTFIX%%.Therefore,  they  all  share  t*
>%%LINK%%[[#^o3bra2053c7|show annotation]]
>%%COMMENT%%
>use collections.UserDict to make a custom mapping for a dictionary if you so need to make on for ti
>%%TAGS%%
>
^o3bra2053c7


>%%
>```annotation-json
>{"created":"2025-05-05T18:18:30.618Z","text":"hashability of an object = has \\__hash\\__() and \\__eq\\__()","updated":"2025-05-05T18:18:30.618Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":236037,"end":236324},{"type":"TextQuoteSelector","exact":"An  object  is  hashable  if  it  has  a  hash  code  which  never  changes  during  its  lifetime  (itneeds  a  __hash__()  method),  and  can  be  compared  to  other  objects  (it  needs  an__eq__()  method).  Hashable  objects  which  compare  equal  must  have  the  same  hashcode.","prefix":"dapted from the Python Glossary:","suffix":"2Numeric  types  and  flat  immu"}]}]}
>```
>%%
>*%%PREFIX%%dapted from the Python Glossary:%%HIGHLIGHT%% ==An  object  is  hashable  if  it  has  a  hash  code  which  never  changes  during  its  lifetime  (itneeds  a  __hash__()  method),  and  can  be  compared  to  other  objects  (it  needs  an__eq__()  method).  Hashable  objects  which  compare  equal  must  have  the  same  hashcode.== %%POSTFIX%%2Numeric  types  and  flat  immu*
>%%LINK%%[[#^1qa44lubcz2|show annotation]]
>%%COMMENT%%
>hashability of an object = has \__hash\__() and \__eq\__()
>%%TAGS%%
>
^1qa44lubcz2


>%%
>```annotation-json
>{"created":"2025-05-05T18:23:23.544Z","updated":"2025-05-05T18:23:23.544Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":237404,"end":237581},{"type":"TextQuoteSelector","exact":"User-defined types are hashable by default because their hash code is their id(), andthe  __eq__()  method  inherited  from  the  object  class  simply  compares  the  objectIDs","prefix":" only within one Python process.","suffix":".  If  an  object  implements  a"}]}]}
>```
>%%
>*%%PREFIX%%only within one Python process.%%HIGHLIGHT%% ==User-defined types are hashable by default because their hash code is their id(), andthe  __eq__()  method  inherited  from  the  object  class  simply  compares  the  objectIDs== %%POSTFIX%%.  If  an  object  implements  a*
>%%LINK%%[[#^zr4cwfe7qcm|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^zr4cwfe7qcm


>%%
>```annotation-json
>{"created":"2025-05-05T18:25:25.804Z","text":"dict.setdefaut(param, defaut) is helpful because it does \n\nvalues = dict.get(param,default) \n<any other operations, like values.append(val)>\ndict[param] = values\n\ndoable in 1 line AND quicker because it performs 1 lookup instead of 2  (3 if not found)","updated":"2025-05-05T18:25:25.804Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":243842,"end":243951},{"type":"TextQuoteSelector","exact":"The three lines dealing with occurrences in Example 3-4 can be replaced by a singleline using dict.setdefault","prefix":"normalize the words forsorting.5","suffix":". Example 3-5 is closer to Alex "}]}]}
>```
>%%
>*%%PREFIX%%normalize the words forsorting.5%%HIGHLIGHT%% ==The three lines dealing with occurrences in Example 3-4 can be replaced by a singleline using dict.setdefault== %%POSTFIX%%. Example 3-5 is closer to Alex*
>%%LINK%%[[#^t6v87jq9rwh|show annotation]]
>%%COMMENT%%
>dict.setdefaut(param, defaut) is helpful because it does 
>
>values = dict.get(param,default) 
><any other operations, like values.append(val)>
>dict[param] = values
>
>doable in 1 line AND quicker because it performs 1 lookup instead of 2  (3 if not found)
>%%TAGS%%
>
^t6v87jq9rwh


>%%
>```annotation-json
>{"created":"2025-05-19T20:47:23.059Z","text":"default dictionaries will handle new key creation and instatiaion","updated":"2025-05-19T20:47:23.059Z","document":{"title":"Fluent%20Python.pdf","link":[{"href":"urn:x-pdf:6c0e57d4e55a6ced4ae3ca1cc17e1b51"},{"href":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf"}],"documentFingerprint":"6c0e57d4e55a6ced4ae3ca1cc17e1b51"},"uri":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","target":[{"source":"vault:/devnotes/ML/Languages/Python/prejohned/Fluent%20Python.pdf","selector":[{"type":"TextPositionSelector","start":246179,"end":246312},{"type":"TextQuoteSelector","exact":"iven a defaultdict created as dd = defaultdict(list), if 'new-key'is not in dd, the expression dd['new-key'] does the following steps","prefix":"tent key argument.For example, g","suffix":":1. Calls list() to create a new"}]}]}
>```
>%%
>*%%PREFIX%%tent key argument.For example, g%%HIGHLIGHT%% ==iven a defaultdict created as dd = defaultdict(list), if 'new-key'is not in dd, the expression dd['new-key'] does the following steps== %%POSTFIX%%:1. Calls list() to create a new*
>%%LINK%%[[#^ez7qt7ba43k|show annotation]]
>%%COMMENT%%
>default dictionaries will handle new key creation and instatiaion
>%%TAGS%%
>
^ez7qt7ba43k
