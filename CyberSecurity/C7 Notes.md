# Automate Cyberscurity Tasks with Python
# Module 1
> ## Programming
> Used to create a specific set of insturctions for a computer to execute tasks
>
> ## Automation
> The use of technology to reduce human and manual effeor to perform common and repetitive tasks
>
> ### Advantages of Python
> - Resembles human language
> - Requires Less code
> - Easy to read
> - Standard guidelines
> - Online support
> - Built-in code
>
> ## Python
> Python is a general purpose programming language that can be used to solve a variety of problems. For example, it can be used to build websites, perform data analysis, and automate tasks. 
>
>Python code must be converted through an interpreter before the computer can process it. An interpreter is a computer program that translates Python code into runnable instructions line by line. 
>
> ### Python in Cybersecurity
> Python is used in cybersecurity especially for automation. \
Some areas of cybersecurity in which Python might be used to automate specific tasks: \
> - Log analysis
> - Malware analysis
> - Access control list management
> - Intrusion detection
> - Compliance checks
> - Network scanning
>
> ## Comment
> A note programmers make about the intention behind their code \
> Syntax: starts with `#` \
> Example: `# Print hello python`
>
> ### print()
> Outputs a specified object tot he screen \
> Syntax:  `print(<value>)` \
> Example: `print("Hello")` \
> **Note**: Strings need to be placed in quotation marks (`"`) 
>
> #### Basic program example
> ```
> # Print Hello Python program
> print("Hello Python!")
>```
>
> ## Python environments
> You can run Python through a variety of environments. These environments include notebooks, integrated development environments (IDEs), and the command line. 
>
> ### Notebooks
> A notebook is an online interface for writing, storing, and running code. They also allow you to document information about the code. Notebook content either appears in a code cell or markdown cell.
> 
> #### Code cells
> Code cells are meant for writing and running code. A notebook provides a mechanism for running these code cells. Often, this is a play button located within the cell. When you run the code, its output appears after the code. 
>
> #### Markdown cells
> Markdown cells are meant for describing the code. They allow you to format text in the markdown language. 
>
> ### Integrated development environments (IDEs)
> Another option for writing Python code is through an integrated development environment (IDE), or a software application for writing code that provides editing assistance and error correction tools. Integrated development environments include a graphical user interface (GUI) that provides programmers with a variety of options to customize and build their programs. 
>
> ### Command line
> Command-line interface (CLI) is a text-based user interface that uses commands to interact with the computer. By entering commands into the command line, you can access all files and directories saved on your hard drive, including files containing Python code you want to run. You can also use the command line to open a file editor and create a new Python file.
>
> ## Data Types in Python
> Category for a particular type of data item
> - #### String data
> Data consisting of an ordered sequence of characters \
> Syntax : `"<string_here>"`
> *Examples*: `"hello", "this is it", ""`.
>> ***Note***: `""` is called an empty string
>
> - #### Float data
> Data consisting of a number with a decimal point. \
> *Example*: 5.6,10.2,-200.3,-0.34,0.0
>
> - #### Integer data
> Data consisting of a number that does not include a decimal point \
> *Example*: -6,12,-200,0,32100,480398423
>
> - #### Boolean data
> Data that can only be one of two values: either True or False
>
> - #### List data
> Data structure that consists of a collection of data in sequential form \
> Syntax: `[value1,value2,...]`
> *Example*:
>```
>[12, 36, 54, 1, 7]
>["eraab", "arusso", "drosas"]
>[True, False, True, True]
>[15, "approved", True, 45.5, False]
>[]
>```
>> ***Note***: `[]` is called an empty list
>
> - #### Tuple
> Tuple data is a data structure that consists of a collection of data that cannot be changed. Like lists, tuples can contain elements of varying data types. \
> Syntax: `(<value1>,<value2>,...)` \
> *Examples*:
> ```
> ("wjaffrey", "arutley", "dkot")
> (46, 2, 13, 2, 8, 0, 0)
> (True, False, True, True)
> ("wjaffrey", 13, True)
>```
>
> - #### Dictionary
> Dictionary data is data that consists of one or more key-value pairs. Each key is mapped to a value. A colon (:) is placed between the key and value. Commas separate key-value pairs from other key-value pairs. \
> Syntax: `{key1: value 1, key2: value2, ...}` \
> Dictionaries are useful when you want to store and retrieve data in a predictable way. For example, the following dictionary maps a building name to a number. The building name is the value, and the number is the key. A colon is placed after the key. \
> *Example*:
> `{ 1: "East", 2: "West",  3: "North",  4: "South" }`
>
> - #### Set data
> In Python, set data is data that consists of an unordered collection of unique values. This means no two values in a set can be the same. \
> Elements in a set are always placed within curly brackets and are separated by a comma. These elements can be of any data type. \
> This example of a set contains strings of usernames: `{"jlanksy", "drosas", "nmason"}`
>
> ## Variables
> A container that stores data
>
> ### type()
> Returns the data type of its input \
> Syntax: `type(<variable>)`
> 