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