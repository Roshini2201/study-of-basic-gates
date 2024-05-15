## EX.NO:1
## DATE:

### study-of-basic-gates

**AIM:** 

To study and verify the truth table of logic gates in Quartus II using Verilog programming.

**Equipments Required:**

Software – Quartus prime 

**Theory**

Introduction Logic gates are the basic building blocks of any digital system. Logic gates are electronic circuits having one or more than one input and only one output. The relationship between the input and the output is based on a certain logic. Based on this, logic gates are named as

AND gate OR gate NOT gate NAND gate NOR gate Ex-OR gate Ex-NOR gate

**AND gate**

The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB
Y= A.B

**OR gate** 

The OR gate is an electronic circuit that gives a high output (1) if one or more of its inputs are high. A plus (+) is used to show the OR operation.
Y= A+B

**NOT gate**

The NOT gate is an electronic circuit that produces an inverted version of the input at its output. It is also known as an inverter. If the input variable is A, the inverted output is known as NOT A. This is also shown as A' or A with a bar over the top, as shown at the outputs.
Y= A'

**NAND gate**

This is a NOT-AND gate which is equal to an AND gate followed by a NOT gate. The outputs of all NAND gates are high if any of the inputs are low. The symbol is an AND gate with a small circle on the output. The small circle represents inversion.
Y= (AB)’

**NOR gate**

This is a NOT-OR gate which is equal to an OR gate followed by a NOT gate. The outputs of all NOR gates are low if any of the inputs are high. The symbol is an OR gate with a small circle on the output. The small circle represents inversion.
Y= (A+B)’

**Ex-OR gate**

The 'Exclusive-OR' gate is a circuit which will give a high output if either, but not both of its two inputs are high. An encircled plus sign (⊕) is used to show the Ex-OR operation.
Y= A⊕B

**Ex-NOR gate**

The 'Exclusive-NOR' gate circuit does the opposite to the EX-OR gate. It will give a low output if either, but not both of its two inputs are high. The symbol is an EX-OR gate with a small circle on the output. The small circle represents inversion.
Y= A⊕B

**Procedure** 

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.

**PROGRAM**

**NAME : ROSHINI S**  
**REGISTER NUMBER : 212223240142**

## AND GATE

**PROGRAM**
```
module and12(a,b,c); 
    input a; 
    input b; 
    output c; 
    assign c = a & b; 
endmodule 
```
 
**Logic symbol & Truthtable**

![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/911b489f-3174-4859-82e3-2843aae4fdc3)



**RTL**
![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/fd976b82-3257-4cdb-8b52-a68e3810417b)



**RTL realization Output:** 

![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/ca7fb055-d49c-4136-b423-c534d365c69d)


## OR GATE

**PROGRAM**
```
module orgate(a,b,d); 
    input a; 
    input b; 
    output d; 
    assign d = a | b; 
endmodule 
```

**Logic symbol & Truthtable**

![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/4590d533-c2d4-42f3-841c-72b3a997c393)



**RTL**

![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/95dc34d9-f505-4002-8e97-80e310256cdc)



**RTL realization Output:** 

![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/82f86db4-3cf3-4ecb-87f5-933a0a759d15)


## NOT GATE

**PROGRAM**
```
module notgate(a,g); 
    input a; 
    output g; 
    assign g = ~a; 
endmodule  
```

**Logic symbol & Truthtable**

![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/4377a3f8-5709-40be-9c66-60c6ece90b6c)



**RTL** 


![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/d188ae6a-390f-4527-a7c1-a8a5c697cb66)


**RTL realization Output:**

![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/5bd53fba-e6a6-4785-b9b3-ab86f63e943c)


## NAND GATE

**PROGRAM**
```
module nandgate(a,b,e);  
input a;  
input b;  
output e; 
assign e = ~(a & b);  
endmodule
```

**Logic symbol & Truthtable**

![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/40bc27e7-2e00-4925-b2b5-7938eee39676)



**RTL**

![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/5fa912fb-8888-47bb-9396-fd8d29ba454a)



**RTL realization Output:**

![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/0c833096-1ed9-41e2-94b0-77e99b46506d)


## NOR GATE

**PROGRAM**
```
module norgate(a,b,f); 
 input a; 
 input b; 
 output f;
 assign f = ~(a | b);
 endmodule 
```
**Logic symbol & Truthtable**

![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/5ad51a9d-69ed-4f91-8fc7-7614f79b31d0)


**RTL**

![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/7eefb84f-8afa-4522-810a-4aaa381474d8)



**RTL realization Output:**

![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/2cbd4445-3f53-46ab-a11c-0c054188af5d)



## EX-OR GATE 

**PROGRAM**
```
module xorgate(a,b,h); 
 input a; 
input b; 
output h; 
assign h = a^ b; 
endmodule
```
**Logic symbol & Truthtable**

![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/cd7dfb25-bbbb-4619-844d-9f342a053707)



**RTL** 

![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/fe097349-ff0a-4f97-a70f-f9bae5fd49fe)

**RTL realization Output:**

![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/70ee70ad-7de4-40f2-b515-0d03349f7ef6)


## EX-NOR

**PROGRAM**
```
module xnorgate(a,b,i);  
input a; 
input b; 
output i; 
assign i = ~(a ^ b); 
endmodule 
```
**Logic symbol & Truthtable**

![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/3f566daa-b6fb-4c51-af68-120ac87b2bc6)



**RTL**

![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/fcd52932-f098-4e9a-93bf-55f6551ada9b)


**RTL realization Output:** 
![image](https://github.com/Roshini2201/study-of-basic-gates/assets/154105318/19215e27-08d6-4629-9466-2dc49afbb9bd)

**RESULT**
Thus,truth table of logic gates in Quartus II using Verilog programming is executed successfully and verified.
