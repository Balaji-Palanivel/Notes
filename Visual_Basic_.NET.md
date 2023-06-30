

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
                                                                                        Visual Basic .NET
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


 -> VB.NET, also known as Visual Basic .NET, is a programming language developed by Microsoft. 
 -> It is an object-oriented programming (OOP) language and is part of the .NET framework.
 -> VB.NET combines the simplicity of the original Visual Basic with the power and flexibility of the .NET framework. 
 -> It supports features such as garbage collection, structured exception handling, multithreading, and interoperability with other .NET languages.


Basic Syntax 
--------------------------------------------------------------------------------------------

Imports System                                                      // Namespace Declaration
Module Hello_Program                                                // Module Name 
    Sub Main()                                                      // Sub Procedure 
  
        Console.WriteLine("Hello, Welcome to the world of VB.NET")  
        Console.WriteLine("Press any key to continue...")   
  
    End Sub                                                         // End of Sub Procedure
End Module                                                          // End of Module


Run Application
--------------------------------------------------------------------------------------------

/> vbc file_name.vb  (OR)  Click - F5


Data Types
--------------------------------------------------------------------------------------------

 -> Boolean                  ->  Byte
 -> Char                     ->  Integer
 -> String                   ->  Long
 -> Double                   ->  Date
 -> Object                   ->  Decimal

VB.NET Methods
-------------------------------------------------------------------------------------------

    --> Main()        -- Gate of program
    --> GetAwaiter()  -- Its used when i use Async function
    --> GetResult()   -- Its used when i use Async function
    --> DirectCast()  -- Its convert objcet to given type


Variable Declaration 
--------------------------------------------------------------------------------------------

Dim Variable_Name As Data_Type  = VALUE          // Using DIM

             (or)

Dim Variable_Name As Data_Type
Variable_Name = VALUE

Const Variable_Name As Data_Type  = VALUE        // Using CONST
Static Variable_Name As Data_Type  = VALUE       // Using Static
Public Variable_Name As Data_Type  = VALUE       // Using Public (or) Private (or) Protected

  --------------------------
 |      Local Variable      |
 |      Module Variable     |  --> Types of variable declarations
 |      Global Variable     |
  --------------------------


Operators  
--------------------------------------------------------------------------------------------

Arithmetic Operators
--------------------
    -->  + (Addition) , - (Subraction) , * (Multiplication) 
    -->  ^ (Power) , / (Division - its returns float value)
    -->  \ (Division - its returns Integer value) , MOD (its returns emainder  value)

Comparision Operators
---------------------
    --> = (Equal) , <> (Not Equal) , > (Greater Then) , < (Less Then) 
    --> >= (Greater Then and equal) , <= (Less Then and equal)
    --> Is (I check both values are same ) , IsNot (Its a opposite for 'Is') 
    --> Like (Its also same as 'Is')

Logical Operator
----------------
    --> And - (True , True = True)    
    --> Or -  (True , False = True)
    --> Not  - Reverse the logical condition
    --> Xor - (True , True = True | False , False = True)
    --> AndAlso - (True , True = True)
    --> OrElse - (True , False = True)

Concatenation Operators
-----------------------
    --> &
    --> +

Miscellaneous Operators
-----------------------
    --> Await
    --> Address Of
    --> Nothing
    --> TypeOf
    --> GetType
    --> Function Expression (like, Lambda function)
    --> If (Like, Terinory operator) -- [Syntax - If(Condition,True statement,False Statement)]


Control Statements  
--------------------------------------------------------------------------------------------

    --> If .. Then 
        ---
        End If

    --> If .. Then 
        --- 
        Else 
        --- 
        End If

    --> If .. Then 
        --- 
        Else If .. Then 
        --- 
        End If

    --> Select Case Expression 
            Case ..
            Case ..
        End Select

    --> Select Case Expression
            Select Cse Expression
                Case ..
                Case ..
                Case ..
            End Select
        End Select


Loop Statements
-------------------------------------------------------------------------------------------

Do Loop
-------------------------------------
    --> Do                           |
                                     |
        ** code **                   | --> Do loop & while
                                     |
        Loop While [Condition]       |
                                    
    --> Do                           |
                                     |
        ** code **                   | --> Do loop & Until
                                     |
        Loop Until [Condition]       |

    --> Do

        ** code **

            Do                           |
                                         |
            ** code **                   | --> Nested Do loop
                                         |
            Loop While [Condition]       |

        Loop While [Condition]

For Next Loop
-------------------------------------
    --> For Variable_Name As Data type = Start_Value to End_Value [Step (i)]       
                                                                                   
            ********                                                                 
                                                                                   
        Next                                                                       
              

For Each Loop
--------------------------------------

    --> For Each Variable_Name As Data_Type In Collection_of_values                
                                                                                   
            *****                                                                  
                                                                                   
        Next                                                                       


While Loop
-------------------------------------

    --> While [Condition]

            ****

        End While

With 
--------------------------------------

    --> With [Object_Value]

            *****

        End With


Exit Statement 
-------------------------------------------------------------------------------------------

    --> Exit [For ,While ,Do , Sub , Function] - The block will be get terminated depends on the condition.

         --------------------------------------------------
        |      If [condition] Then                         |
        |       Exit [For ,While ,Do , Sub , Function]     |  
        |      Global Variable                             |
         --------------------------------------------------


Continue Statement
-------------------------------------------------------------------------------------------

    --> Continue [For , While , Do]  - block will be get skip depends on the condition.

         --------------------------------------------------
        |      If [condition] Then                         |
        |       Continue [For ,While ,Do]                  |  
        |      Global Variable                             |
         --------------------------------------------------


GoTo Statement
-------------------------------------------------------------------------------------------

--> GoTo Lable_Name  - Its help to redirect the program depend on the condition.

         --------------------------------------------------
        |      If [condition] Then                         |
        |       GoTo Odd                                   |  
        |      Global Variable                             |
        |   Odd:                                           |
        |      console.write("Odd)                         |
        |   Even:                                          |
        |      console.write("Even")                       |
         --------------------------------------------------


Enum
-------------------------------------------------------------------------------------------


    --> Enum  -  Used to define a related set of constants as a list using the keyword enum.

         --------------------------------------------------
        |      Enum                                        |
        |        Variable_1                                |  
        |        Variable_2                                |
        |        Variable_3                                |
        |      End Enum                                    |
         --------------------------------------------------


String 
-------------------------------------------------------------------------------------------

    --> String  -  String is a collection of charecters

String Methods
-------------------------

    --> Split()                                        
    --> Length                                         
    --> Contains()
    --> ToUpper()
    --> ToLower()
    --> StartsWith()
    --> EndsWith()
    --> Trim()
    --> Replace()     - (As String , As String)
    --> Compare()     - (As String , As String)
    --> Concat()      - (As String , As String)
    --> Copy()        
    --> CopyTo()      - (SourceIndex , CharArray , DesinationIndex , Length)
    --> Equals()      - (As String , As String)
    --> Format()
    --> IndexOf()
    --> Insert()      - (InsertPosition , As String)
    --> Remove()      - (RemovePosition)
    --> Join()        - (As String , As String)



ArrayList
-------------------------------------------------------------------------------------------

    --> ArrayList  -  Its used to store and retrive collection of objects, Its like a Array.

ArrayList Methods
-------------------------

    --> Add()             - Add a new elements to ArrayList                 [ArrayList.Add("Apple")]
    --> Remove()          - Remove a elemnet from ArrayList                 [ArrayList.Remove("Apple")]
    --> Insert()          - Insert a element to ArrayList at specifi Index  [ArrayList.Insert(8,"Apple")]
    --> Contains()        - Its check arguement is have or not in ArrayList [ArrayList.Contains("Apple")]
    --> Clear()           - To clear all elements from ArrayList            [ArrayList.Clear()]
    --> Sort()            - To Sort an ArrayList                            [ArrayList.Sort()]
    --> Count             - To Count the total elements of ArrayList        [ArrayList.Count]
    --> Capacity          - To set a initial capacity od ArratList          [ArrayList.Capacity = 10]
    --> RemoveAt()        - To Remove specific element from ArrayList       [ArrayList.Remove(8,"Apple")]
    --> RemoveRange()     - To remove one or more elements from ArrayList   [ArrayList.RemoveRange(2,5)]
    --> InsertRange()     - To insert one or more elements to ArrayList     [ArrayList.InsertRange(1, New List(Of String)() From {"Banana", "Orange"})]



HashTable
--------------------------------------------------------------------------------------------

    --> HashTable  -  A HashTable is used to store the collection of different types of data in key-value pairs. 

HashTable Methods
-------------------------

    --> Add()                            --> Count
    --> Remove()                         --> Item
    --> clear()                          --> Keys
    --> ContainsKey()                    --> Values
    --> ContainsValue()                  --> Keys
    --> GetHash()                        --> IsFixedSize
                                         --> IsSynchronized 
                                         --> IsReadOnly
    

Stack
----------------------------------------------------------------------------------------------

    --> Stack  -  The stack is a homogeneous collection of elements used to store elements based on LIFO (Last-In First-Out). 

Stack Methods
------------------------

    --> Push()
    --> Pop()
    --> Peek()
    --> Contains()
    --> Clear()
    
Queue
----------------------------------------------------------------------------------------------

    --> Stack  -  The Oueue is a  collection of elements used to store elements based on FIFO (Last-In First-Out). 

Queue Methods
------------------------

    --> EnQueue()
    --> DeQueue()
    --> Peek()
    --> Contains()
    --> Clear()


Array
---------------------------------------------------------------------------------------------

    --> Array  -  Array is collection of data with same data types.

         --------------------------------------------------
        |                                                  |
        |  Dim Array_Name() As Data_Type = {1,2,3,4,5}     |  
        |                                                  |
        |  Dim Array_Name() As Data_Type = New Integer(){} |
        |                                                  |
        |  Dim Array_Name(5) As Data_Type                  |
        |                                                  |
        |  Dim Emp(0 to 2) As String                       |
        |     Emp{0} = "Mathew"                            | 
        |     Emp(1) = " Anthony"                          |
        |                                                  |
         --------------------------------------------------

MultiDimentional Array
-----------------------

    --> Two Dimentioanl Array
        ---------------------

          -----------------------------------------------------
        |                                                      |
        |  Dim Array_Name(,) As Data_Type = {{00,01},{10,11}}  |  
        |                                                      |
         ------------------------------------------------------

    --> Three Dimentioanl Array
        -----------------------

          ----------------------------------------------------
        |                                                     |
        |  Dim Array_Name(,,) As Data_Type = {{{1,2},{3,4}},  |
        |                                     {{5,6},{7,8}},  |
        |                                     {{9,4},{5,6}}}  |  
        |                                                     |
         -----------------------------------------------------
   
    --> Dynamic Array
        ----------------

        In Dynamic Array we use 'ReDim' and 'Resize' statement to resize a array.

         --------------------------------------------------
        |                                                  |
        |  Dim Array_Name() As Data_Type = {1,2,3,4,5}     |  
        |                                                  |
        |  *** code ***                                    |
        |                                                  |
        |  ReDim Preserve Array_Name(7)                    |
        |                                                  |
        |  Array_Name.(6) = 6                              |
        |  Array_Name.(7) = 7                              |
        |                                                  |
         --------------------------------------------------



NameValueCollection
----------------------------------------------------------------------------------------

    --> NameValueCollection  -  It is similer to HashTable. Its collection of key/value pairs.

    NameValueCollection Methods
    ---------------------------

        --> Get()
        --> GetValue()
        --> Add()
        --> Remove()
        --> Clear()
        --> Equals()
        --> Set()


List
----------------------------------------------------------------------------------------

    --> List  -  It is a collection of objects .

    List Methods
    ---------------------------

        --> Add()
        --> Remove()
        --> RemoveAt()
        --> Clear()
        --> Contains()
        --> Sort()
        --> Count
        --> IndexOf()


File Handling
---------------------------------------------------------------------------------------

    Class Names
    ----------------------

        --> FileStream
        --> StreamWriter
        --> StreamReader
        --> BinaryWriter
        --> BinaryReader
        --> FileInfo
        --> DirectoryInfo
        
