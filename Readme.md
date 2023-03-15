<a name="_1z15jug079jg"></a>**Lab 5**

<a name="_ksi5d8hv6p9m"></a>Keshav Somani 				    	 202001029

#
# <a name="_4163mzsexsd8"></a><a name="_8iwc7u9we3nm"></a>Erroneous code 1: 
### <a name="_hhfxdcwuze7w"></a>**SOURCE** : Bing-Chatgpt 
The source of the code is Bing Chat.

![](Aspose.Words.950ede93-08b8-4e20-a657-9fcbf9b560dc.001.png)

On asking Bing-Chat : 




It returns for the code :

\# pylint: disable=missing-module-docstring

import argparse

import sys

from pylint import lint

desc = "Run pylint with a threshold for score"

parser = argparse.ArgumentParser(description=desc, allow\_abbrev=False)

parser.add\_argument(

`    `"--fail-under",

`    `dest="threshold",

`    `type=float,

`    `default=8,

`    `help="If the final score is more than THRESHOLD, exit with"

`    `" exitcode 0, and pylint's exitcode otherwise.",

)

args, remaining\_args = parser.parse\_known\_args()

threshold = args.threshold

run = lint.Run(remaining\_args, do\_exit=False)

score = run.linter.stats["global\_note"]

if score < threshold:

`    `sys.exit(run.linter.msg\_status)





## <a name="_8sk1wvj928zc"></a>Static-Analysis using Pylint :
We had Installed Pylint Extension in VS-Code  

![](Aspose.Words.950ede93-08b8-4e20-a657-9fcbf9b560dc.002.png)

Created a **test.py** and imported the erroneous code in it 











## <a name="_x85ynjfbbxf4"></a>Output:
**Problems :** Pylint can identify the problems in the code.

![](Aspose.Words.950ede93-08b8-4e20-a657-9fcbf9b560dc.003.png)


**Indentation :** Pylint also identifies Bad - Indentation.![](Aspose.Words.950ede93-08b8-4e20-a657-9fcbf9b560dc.004.png)






















**Suggestions :** It also shows suggestions for better code writing and overall understandability of code. 

![](Aspose.Words.950ede93-08b8-4e20-a657-9fcbf9b560dc.005.png)





# <a name="_2sdmhlf6hi53"></a>Erroneous Code 2:
**Source Code: <https://github.com/andy-landy/traceback_with_variables.git>** ->: examples folder

**Change\_global\_printer.py**

def main():

`    `n = 0

`    `print(1 / n)


main()


