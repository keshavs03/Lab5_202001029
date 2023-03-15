<a name="_1z15jug079jg"></a>**Lab 5**

<a name="_ksi5d8hv6p9m"></a>Keshav Somani 				    	 202001029

#































## <a name="_7a31l95ccj59"></a><a name="_8sk1wvj928zc"></a>Static-Analysis using Pylint :
We had Installed Pylint Extension in VS-Code  

![](Aspose.Words.a7958bc7-00d8-4720-b18f-e5900e45bbf3.001.png)

Created a **test.py** and imported the erroneous code in it 








# <a name="_8iwc7u9we3nm"></a>Erroneous code 1: 
### <a name="_hhfxdcwuze7w"></a>**SOURCE** : Bing-Chatgpt 
The source of the code is Bing Chat.

![](Aspose.Words.a7958bc7-00d8-4720-b18f-e5900e45bbf3.002.png)

On asking Bing-Chat : 




It returns for the code :

![](Aspose.Words.a7958bc7-00d8-4720-b18f-e5900e45bbf3.003.png)





















## <a name="_x85ynjfbbxf4"></a>Output:
**Problems :** Pylint can identify the problems in the code.

![](Aspose.Words.a7958bc7-00d8-4720-b18f-e5900e45bbf3.004.png)


**Indentation :** Pylint also identifies Bad - Indentation.![](Aspose.Words.a7958bc7-00d8-4720-b18f-e5900e45bbf3.005.png)






















**Suggestions :** It also shows suggestions for better code writing and overall understandability of code. 

![](Aspose.Words.a7958bc7-00d8-4720-b18f-e5900e45bbf3.006.png)





# <a name="_2sdmhlf6hi53"></a>Erroneous Code 2:
**Source Code: <https://github.com/andy-landy/traceback_with_variables.git>** ->: examples folder

**Change\_global\_printer.py**

![](Aspose.Words.a7958bc7-00d8-4720-b18f-e5900e45bbf3.007.png)















## <a name="_8u2zduqzli7m"></a>Output:
**Missing Line:** Pylint is able to identify Missing-Lines / words.

![](Aspose.Words.a7958bc7-00d8-4720-b18f-e5900e45bbf3.008.png)


# <a name="_30wn03q78850"></a>Analysis:
After testing over Erroneous Code 1 & 2. We can see multiple errors identified by Pylint .

Now we will analysis the output on the basis of correct detection and incorrect detection:

## <a name="_8uph9x4mjdud"></a>Correct Detection :

1. ### <a name="_1zotpm37b6g9"></a>Is - Error Detected
In Code 1 we can see multiple output , and can analyze that Pylint can successfully detect errors that are 

- Miscellaneous Typing 
- Wrong function / command written
- Indentation Errors 


## <a name="_m8xymgxn23gt"></a>Incorrect Detection :
1. ### <a name="_t6duf0q5e071"></a>Is - Error Undetected:
In Code 2 we can see the function was asking to run command (1/0) which is mathematically invalid. Therefore , we can analyze that Pylint is unable to detect 

- Mathematically wrong codes
- Stuck in Loop Problems
1. ### <a name="_9dmzkl4l7hff"></a>Not- Error Detected:
In Code 2 we can see the function was unable to differentiate between Globally Pre-Defined and Defining functions



