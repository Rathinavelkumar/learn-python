The top must known inbuilt function in python are

## **Abs Function**
Abs function helps to return the absolute value of given number

    #Abs Function
    input_value = -50

    output_value = abs(input_value)
    print(output_value)

 Output

    50

## **All Function**
All function checks all the elements in the given iterable is true or not

    #All Function
    input_value = [10, 20, 30, 40]

    output_value = all(input_value)
    print(output_value)

 Output

    True

Zero or False value in the given input returns false

    #All Function
    input_value = [10, 20, 30, 0]

    output_value = all(input_value)
    print(output_value)

 Output

    False

## **Any Function**
Any function returns true if any one of the element is true in given iterable

    #Any Function
    input_value = [10, 20, 30, 0]

    output_value = any(input_value)
    print(output_value)

 Output

    True

## **ASCII(Ord) Function**
Ord function helps to return the ASCII (American Standard Code for Information value of given character Interchange)

    #Ord Function
    input_value = "R"

    output_value = ord(input_value)
    print(output_value)

 Output

    82

## **Bin Function**
Bin function helps to convert the decimal number to a binary string. Result have `ob` prefix which indicates the binary format

    #Bin Function
    input_value = 10

    output_value = bin(input_value)
    print(output_value)

 Output

    0b1010

## **Bool Function**
Bool functions returns the Boolean value (i.e.) either true or false

    #Bool Function
    input_value1 = 0
    input_value2 = 1

    output_value1 = bool(input_value1)
    print(output_value1)

    output_value2 = bool(input_value2)
    print(output_value2)

 Output

    False
    True

## **Breakpoint Function**
In python 3.7, breakpoint function has introduced which helps to invoke breakpoint without import of pdb module. Previously we can use the pdb module, in which pdb.set_trace() function act as a breakpoint

    #Breakpoint Function
    input_value1 = 0
    input_value2 = 1

    output_value1 = bool(input_value1)
    print(output_value1)


    output_value2 = bool(input_value2)
    print("Want to continue? Press c and Enter")
    breakpoint()
    print(output_value2)

 Output

    False
    Want to continue? Press c and Enter
    > <string>(12)<module>()
    (Pdb) c
    True

## **Bytearray Function**
As per python documentation, Bytearray function Return a new array of bytes. The bytearray type is a mutable sequence of integers in the range 0 < x < 256.

**source [optional]: byte array initializer**

**encoding [optional]: string encoding method**

**errors [optional]: steps to perform during failure of encoding**

    #ByteArray Function
    input_data = "RATHNA SCHOOLS"

    output1 = bytearray(input_data, "utf-8")
    print(output1)

    output2 = bytearray(input_data, "utf-16")
    print(output2)

 Output

    bytearray(b'RATHNA SCHOOLS')
    bytearray(b'\xff\xfeR\x00A\x00T\x00H\x00N\x00A\x00 \x00S\x00C\x00H\x00O\x00O\x00L\x00S\x00')

## **Bytes Function**
Byte function is similar to bytearray but they returns a immutable bytes object, so it cannot be changed once declared

    #Bytes Function
    input_data = "RATHNA SCHOOLS"

    output1 = bytes(input_data, "utf-8")
    print(output1)

    output2 = bytes(input_data, "utf-16")
    print(output2)

 Output

    b'RATHNA SCHOOLS'
    b'\xff\xfeR\x00A\x00T\x00H\x00N\x00A\x00 \x00S\x00C\x00H\x00O\x00O\x00L\x00S\x00'

## **Callable Function**
Callable function helps to check whether the given object argument is callable or not

    #Function1
    def add():
        return "add function"
        
    #Function2
    def sub():
        return "sub function"
        
    #Variable
    mul = "mul function"
        
    print(callable(add))
    print(callable(sub))
    #Its variable, not a callable function
    print(callable(mul))

 Output

    True
    True
    False

## **Chr Function**
Chr function helps to convert the ASCII value to its original character 

    #Chr Function
    input_data = "R"

    #convert to ASCII value
    output_value1 = ord(input_data)
    print(output_value1)

    #Convert back to original character
    output_value2 = chr(output_value1)
    print(output_value2)

 Output

    82
    R

## **Compile Function**
Compile method helps to convert the source code to an executable, so that it can execute whenever required

**syntax - compile(source, filename, mode)**

**source - source code (it can single line or complete block**

**filename - source code reading filename, if not we can pass random name**

**mode - eval mode in case of single line, exec can use for multi line source code**

    #Compile Function
    source_code = "print('RATHNA SCHOOLS')"

    compile_code = compile(source_code, "Test", "eval")

    eval(compile_code)

 Output

    RATHNA SCHOOLS

## **Complex Function**
Complex function used to covert the string or number into a complex number 

    #Complex Function
    input_data1 = complex(5,10)
    print(input_data1)

    input_data2 = complex(5)
    print(input_data2)

 Output

    (5+10j)
    (5+0j)

## **Deltattr Function**
Deltattr function helps to delete the named attribute from the given object which should be allows it

    #Delattr Function
    class Score:
        python = 100
        js = 90
        java = 80
        
    #Object Creation
    score_object = Score()

    #Before Deletion
    print(score_object.python)
    print(score_object.js)
    print(score_object.java)

    #After Deletion
    delattr(Score, 'java')
    print(score_object.python)
    print(score_object.js)
    print(score_object.java)

 Output

    100
    90
    80
    100
    90
    Traceback (most recent call last):
    File "<string>", line 19, in <module>
    AttributeError: 'Score' object has no attribute 'java'

## **Dict Function**
Dict Function helps to create a new dictionary

    #Dict Function
    input_dict = dict(
        Name = "Rathna Schools",
        Language = "Python"
        )

    print(input_dict)

 Output

    {'Name': 'Rathna Schools', 'Language': 'Python'}

## **Dir Function**
Dir function is one of the most important built-in function in python.

without parameter -  It helps to return the list of name in current local scope

with parameter - it helps to list the valid methods of given object in current local scope 

    #Dir Function
    print("Without parameter")
    print(dir())

    print("With Parameter")
    input_data = list()
    print(dir(input_data))

 Output

    Without parameter
    ['__annotations__', '__builtins__', '__doc__', '__loader__', '__name__', '__package__', '__spec__']
    With Parameter
    ['__add__', '__class__', '__contains__', '__delattr__', '__delitem__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__getitem__', '__gt__', '__hash__', '__iadd__', '__imul__', '__init__', '__init_subclass__', '__iter__', '__le__', '__len__', '__lt__', '__mul__', '__ne__', '__new__', '__reduce__', '__reduce_ex__', '__repr__', '__reversed__', '__rmul__', '__setattr__', '__setitem__', '__sizeof__', '__str__', '__subclasshook__', 'append', 'clear', 'copy', 'count', 'extend', 'index', 'insert', 'pop', 'remove', 'reverse', 'sort']

