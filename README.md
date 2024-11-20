# FRESH
JAVASCRIPT CODE ASSIGNMENT
var message="Hello";
var Name="feranmi";
var class="ss3";
var university="Redeeemers";
var food="fried rice";
var sport="volleyball";
var game="action";
var sportman="ronaldo";
var cook="hilda";
var app="instagram";
var church="rccg";
var book="isnpiring literature";
var pagenumber="six";
var startdate="may";
var enddate="september";
var productname="milo";
var productprice=6500;
var color="red";
var maagazine="fashion;
var currency="naira";
var input="daily";
var income="monthly";
var engagement="everyday";
var age="18";
var email="none";
var taxrate="increase";
var trading="none";
var teacher="Mr mike";
var class="javascript";
var time="once in a week";
var grade"good";
var textbook="none";
var workbook="none";
var company="upperlink";
var investement="naira";
var home="nice";
var school="Dee Unique";
var position="milfielder";
var age=20;
var portfolio="working";
var city="Ikeja";
var state="lagos";
var country="nigeria";
var continent="africa";
var ="feranmi";
var phone="techno";
var weight="slim";
var haircolor="black"
var eyecolor="brown"
50 NUMBERS
var num1=10;
var num1=11;
var num1=12;
var num1=13;
var num1=14;
var num1=15;
var num1=16;
var num1=17;
var num1=18;
var num1=19;
var num1=20;
var num1=21;
var num1=22;
var num1=23;
var num1=24;
var num1=25;
var num1=26;
var num1=27;
var num1=28;
var num1=29;
var num1=30;
var num1=31;
var num1=32
var num1=33;
var num1=34;
var num1=35;
var num1=36;
var num1=37;
var num1=38;
var num1=39;
var num1=40;
var num1=41;
var num1=42;
var num1=43;
var num1=44;
var num1=45;
var num1=46;
var num1=47;
var num1=48;
var num1=49;
var num1=50;
50 BOOLEAN
var bool1=true
var bool2=false
var bool2=true
var bool2=true
var bool2=true
var bool2=true
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
var bool2=false
10 BigInt
var BigInt1=BigInt("12345678901234567890");
var BigInt2=BigInt("987654321098765432109876543210");
var BigInt3=BigInt("11223344556677889900112233445566778899");
var BigInt4=BigInt("102030405060708090100110120130140150160");
var BigInt5=BigInt("999999999999999999999999999999999999");
var BigInt6=BigInt("100000000000000000000000000000000000000000");
var BigInt7=BigInt("3141592653589793238462643383279502884197");
var BigInt8=BigInt("2718281828459045235360287471352662497757");
var BigInt9=BigInt("161803398874989484820458683436563811772");
var BigInt10=BigInt("1414213562373095048801688724209698078569");
ASSIGNMENT ON BIGINT
In JavaScript, numbers are typically represented using the Number type, which is a 64-bit floating point value, adhering to the IEEE 754 standard. This works well for most applications, but there are certain limitations. For example, the largest safe integer in JavaScript that can be accurately represented is 2^53 - 1, or 9,007,199,254,740,991. Numbers beyond this value can lose precision, causing unexpected behavior in applications dealing with very large integers.
To overcome this limitation, JavaScript introduced the BigInt type in ECMAScript 2020 (ES11). A BigInt allows developers to work with integers beyond the safe range of the Number type, enabling precise representation and arithmetic for arbitrarily large integers. Let's dive deeper into the key features, usage, and potential pitfalls of BigInt.
What is BigInt?
A BigInt is a built-in object in JavaScript that represents an integer of arbitrary precision. Unlike the Number type, which has fixed precision, BigInt can represent integers as large as the system memory allows. This makes it ideal for applications that need to handle large numbers, such as cryptography, financial applications, and scientific calculations.
The main difference between BigInt and Number is how they handle integers. While Number is based on floating-point arithmetic and has a fixed range and precision, BigInt can grow to any size, storing integers accurately no matter how large.
Creating a BigInt
You can create a BigInt in two ways:
By appending an n at the end of a number literal
Using the BigInt constructor
Arithmetic with BigInt
BigInt supports all the common arithmetic operations such as addition, subtraction, multiplication, and division, just like regular numbers. However, there are a few important nuances to keep in mind
Addition/Subtraction/Multiplication: These work seamlessly with BigInt
Division: Division of BigInt values will truncate any remainder, returning the largest integer less than or equal to the result
Exponentiation: BigInt also supports exponentiation (** operator)
Compatibility with Number
Although BigInt and Number are both used for representing numerical values, they are not directly compatible with each other. You cannot mix them in operations without converting one type to the other.
You cannot mix BigInt with Number
Use Cases for BigInt
Large Numbers: Any domain requiring extremely large integers, such as cryptography or high-precision scientific calculations, benefits from BigInt. For example, when dealing with prime numbers in cryptographic algorithms like RSA, or calculating large factorials in mathematics.
Financial Applications: In financial systems, transactions involving large amounts of money are common, and BigInt allows for accurate and safe calculations involving very large values, ensuring no precision loss in calculations like currency conversions or national debts.
Arbitrary Precision: When performing operations that need to handle numbers beyond the 53-bit limit of JavaScript's Number type, such as in certain algorithms in data science, BigInt is an essential tool.
Pitfalls of BigInt
While BigInt provides useful functionality, there are some limitations and considerations:
Performance: Since BigInt can represent arbitrarily large numbers, operations on BigInt values may be slower than on regular numbers due to the overhead of managing large integer calculations.
Compatibility: As mentioned earlier, BigInt and Number are not directly compatible, which means that careful type conversions are necessary when working with APIs or libraries that expect Number types.
JSON Serialization: BigInt is not natively supported in JSON, meaning that you cannot directly serialize or deserialize BigInt values with JSON.stringify() or JSON.parse(). Workarounds like converting BigInt to strings before serialization are required:
BigInt is a powerful addition to JavaScript that allows developers to work with integers of arbitrary precision. It is useful in situations where the limitations of the Number type are inadequate, such as in high-precision calculations, cryptography, or financial systems. However, it also comes with certain restrictions and performance trade-offs that should be considered when deciding whether to use it. Understanding these differences and how BigInt interacts with other data types is essential for writing robust and efficient JavaScript applications.
