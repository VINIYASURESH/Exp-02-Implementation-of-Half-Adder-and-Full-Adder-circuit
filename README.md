Developed by: VINIYA J B

RegisterNumber:22008831


AIM:To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.


Equipments Required:Hardware – PCs, Cyclone II , USB flasher  Software – Quartus prime


Theory:Adders are digital circuits that carry out addition of numbers.


Half Adder:Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB


Full Adder:Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin


Figure -01 HALF ADDER 

![A](https://user-images.githubusercontent.com/121683551/213443980-2bcfff5d-6243-4aad-b672-ce9b2348af1e.png)


Figure -02 FULL ADDER 

![B](https://user-images.githubusercontent.com/121683551/213444064-8ded00ae-7a3e-4fef-a57c-98d093f98a2f.png)


Procedure:Connect the supply (+5V) to the circuit  Switch ON the main switch   If the output is 1, then the led glows.


Program:Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
  
HALF ADDER

module HalfAdder(a,b,sum,carry); input a,b; output sum,carry; xor(sum,a,b); and(carry,a,b); endmodule

FULL ADDER

module FullAdder(a,b,c,sum,carry); input a,b,c; output sum,carry; assign sum = ((a^b)^c); assign carry = ((a&b)|(b&c)|(c&a)); endmodule

![C](https://user-images.githubusercontent.com/121683551/213444648-2818514f-8508-41bb-b294-3ed8c2c36e9a.png)


Logic symbol 
Output: RTL realization

HALF ADDER

![D](https://user-images.githubusercontent.com/121683551/213445069-8d70443d-96df-4e79-aa30-bde0644843c8.png)


FULL ADDER

![E](https://user-images.githubusercontent.com/121683551/213445109-65eafb53-efb9-4421-a410-7be6a22e281c.png)


TIMING DIAGRAM

HALF ADDER

![F](https://user-images.githubusercontent.com/121683551/213445203-c7ef9c2d-3881-48b8-b34a-7f46e144ab56.png)


FULL ADDER

![G](https://user-images.githubusercontent.com/121683551/213445254-fdd373ad-2541-48c7-807a-bff4e5d6812a.png)


TRUTH TABLE

HALF ADDER

![H](https://user-images.githubusercontent.com/121683551/213445288-ffa619c9-1172-4416-9659-c2b52856af59.png)


FULL ADDER

![H - Copy](https://user-images.githubusercontent.com/121683551/213445342-ed5c7f7a-d5a9-42c9-81a1-e2c624f4fa65.png)



Result: Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
























