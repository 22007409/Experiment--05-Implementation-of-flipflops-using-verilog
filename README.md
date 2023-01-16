Developed by:V SANDHIYA

RegisterNumber:22007409


AIM: To implement all the flipflops using verilog and validating their functionality using their functional tables


HARDWARE REQUIRED:–

PC, Cyclone II , USB flasher


SOFTWARE REQUIRED:-  

Quartus prime


THEORY


SR Flip-Flop


SR flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, SR latch operates with enable signal. The circuit diagram of SR flip-flop is shown in the following figure.


![A1](https://user-images.githubusercontent.com/121559414/212612709-393674b5-059d-40bd-9de7-d8c86876dd05.png)


This circuit has two inputs S & R and two outputs Qtt & Qtt’. The operation of SR flipflop is similar to SR Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable.The following table shows the state table of SR flip-flop.


![A2](https://user-images.githubusercontent.com/121559414/212612794-91c03303-9b85-4116-85ed-49e3a0bacb93.png)


Here, Qtt & Qt+1t+1 are present state & next state respectively. So, SR flip-flop can be used for one of these three functions such as Hold, Reset & Set based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of SR flip-flop.
Present Inputs	Present State	Next State


![A3](https://user-images.githubusercontent.com/121559414/212612877-5e7048f4-2206-4b1f-8263-c24a512dd104.png)


By using three variable K-Map, we can get the simplified expression for next state, Qt+1t+1. The three variable K-Map for next state, Qt+1t+1 is shown in the following figure.


![A4](https://user-images.githubusercontent.com/121559414/212612906-6c512fd3-296d-427a-a719-265ba818790e.png)

 
The maximum possible groupings of adjacent ones are already shown in the figure. Therefore, the simplified expression for next state Qt+1t+1 is
Q(t+1)=S+R′Q(t)Q(t+1)=S+R′Q(t)



D Flip-Flop


D flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, D latch operates with enable signal. That means, the output of D flip-flop is insensitive to the changes in the input, D except for active transition of the clock signal. The circuit diagram of D flip-flop is shown in the following figure.
 
This circuit has single input D and two outputs Qtt & Qtt’. The operation of D flip-flop is similar to D Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable.
The following table shows the state table of D flip-flop.


![A5](https://user-images.githubusercontent.com/121559414/212613024-ca70a343-a991-420d-8093-664913b74293.png)


![A6](https://user-images.githubusercontent.com/121559414/212613049-0f2a32d8-6980-45d9-a09b-04dd2345d3ad.png)


Therefore, D flip-flop always Hold the information, which is available on data input, D of earlier positive transition of clock signal. From the above state table, we can directly write the next state equation as Qt+1t+1 = D


![A7](https://user-images.githubusercontent.com/121559414/212613130-616669cd-1232-4286-9924-b68385a36644.png)


Next state of D flip-flop is always equal to data input, D for every positive transition of the clock signal. Hence, D flip-flops can be used in registers, shift registers and some of the counters.



JK Flip-Flop


JK flip-flop is the modified version of SR flip-flop. It operates with only positive clock transitions or negative clock transitions. The circuit diagram of JK flip-flop is shown in the following figure.


![A8](https://user-images.githubusercontent.com/121559414/212613203-fbc64a63-e34f-43fa-9682-932ed607f784.png)


This circuit has two inputs J & K and two outputs Qtt & Qtt’. The operation of JK flip-flop is similar to SR flip-flop. Here, we considered the inputs of SR flip-flop as S = J Qtt’ and R = KQtt in order to utilize the modified SR flip-flop for 4 combinations of inputs.
The following table shows the state table of JK flip-flop.


![A9](https://user-images.githubusercontent.com/121559414/212613283-d5f57b38-19a7-4965-affb-1ffd72561494.png)


Here, Qtt & Qt+1t+1 are present state & next state respectively. So, JK flip-flop can be used for one of these four functions such as Hold, Reset, Set & Complement of present state based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of JK flip-flop.
Present Inputs	Present State	Next State


![A10](https://user-images.githubusercontent.com/121559414/212613337-e44e5c54-4bae-4757-a7f0-e636a43670ac.png)


By using three variable K-Map, we can get the simplified expression for next state, Qt+1t+1. Three variable K-Map for next state, Qt+1t+1 is shown in the following figure.
 
 
![A11](https://user-images.githubusercontent.com/121559414/212613381-c808f52e-9c80-439d-8ffd-bdd01a6395fa.png)
 
 
The maximum possible groupings of adjacent ones are already shown in the figure. Therefore, the simplified expression for next state Qt+1t+1 is
Q(t+1)=JQ(t)′+K′Q(t)Q(t+1)=JQ(t)′+K′Q(t)



T Flip-Flop


T flip-flop is the simplified version of JK flip-flop. It is obtained by connecting the same input ‘T’ to both inputs of JK flip-flop. It operates with only positive clock transitions or negative clock transitions. The circuit diagram of T flip-flop is shown in the following figure.


![A12](https://user-images.githubusercontent.com/121559414/212613460-d2b4fc7f-ed4e-4a34-8ec6-467613e891fd.png)


This circuit has single input T and two outputs Qtt & Qtt’. The operation of T flip-flop is same as that of JK flip-flop. Here, we considered the inputs of JK flip-flop as J = T and K = T in order to utilize the modified JK flip-flop for 2 combinations of inputs. So, we eliminated the other two combinations of J & K, for which those two values are complement to each other in T flip-flop.The following table shows the state table of T flip-flop.


Here, Qtt & Qt+1t+1 are present state & next state respectively. So, T flip-flop can be used for one of these two functions such as Hold, & Complement of present state based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of T flip-flop.
Inputs	Present State	Next State


![A13](https://user-images.githubusercontent.com/121559414/212613543-b33c6a4d-882b-4674-84d3-1992e6b12d3c.png)


From the above characteristic table, we can directly write the next state equation as Q(t+1)=T′Q(t)+TQ(t)′
⇒Q(t+1)=T⊕Q(t)



PROCEDURE

1.Open Quartus II and select new project and choose the file location.

2.Module Declaration. Module should have the file name.

3.Declare Inputs and outputs.

4.Use assign declaration and wire to define the functionality of logic circuits.

5.End the program with endmodule.

6.Run the program and choose RTL viewer to get RTL realization.



PROGRAM 

Program for flipflops  and verify its truth table in quartus using Verilog programming.


SR FLIP-FLOP
:

```
module SR(S,R,clk,Q,Qbar);  

input S,R,clk;  

output Q,Qbar;  

wire X,Y;  

nand (X,S,clk);  

nand (Y,R,clk);  

nand (Q,X,Qbar);  

nand (Qbar,Y,Q);  

endmodule
```


D FLIP-FLOP
:

```
module DF(D,clk,Q,Qbar);  

input D,clk;  

output Q,Qbar;  

assign Dbar=~D;  

wire X,Y;  

nand (X,D,clk);  

nand (Y,Dbar,clk);  

nand (Q,X,Qbar);  

nand (Qbar,Y,Q);  

endmodule
```


JK FLIP-FLOP
:

```
module JK(J,K,clk,Q,Qbar);  

input J,K,clk;  

output Q,Qbar;  

wire X,Y;  

nand (X,J,clk,Qbar);  

nand (Y,K,clk,Q);  

nand (Q,X,Qbar);  

nand (Qbar,Y,Q);  

endmodule
```


T FLIP-FLOP
:

```
module TF(T,clk,Q,Qbar);  

input T,clk;  

output Q,Qbar;  

wire S,R;  

nand (S,T,clk,Qbar);  

nand (R,T,clk,Q);  

nand (Q,S,Qbar);  

nand (Qbar,R,Q);  

endmodule
```



RTL LOGIC FOR FLIPFLOPS 


SR FLIP-FLOP:

![1A](https://user-images.githubusercontent.com/121559414/212614027-3f41d7e2-4b94-47fc-ad95-0567f547c9fa.png)


D FLIP-FLOP:

![1B](https://user-images.githubusercontent.com/121559414/212614082-f2b09f44-bd3c-4ad3-a1aa-0e0b75a99531.png)


JK FLIP-FLOP:

![1C](https://user-images.githubusercontent.com/121559414/212614160-b9f5701c-6ea2-4d98-893d-525684b73fa8.png)


T FLIP-FLOP:

![1D](https://user-images.githubusercontent.com/121559414/212614260-c29ce6b0-7ed0-47d9-b4db-16a31f59052a.png)



TIMING DIGRAMS FOR FLIP FLOPS:


SR FLIP-FLOP:

![Q1](https://user-images.githubusercontent.com/121559414/212614380-ddb88b8f-ff7e-45bc-89f5-f57f5f2dda7b.png)


D FLIP-FLOP:

![Q2](https://user-images.githubusercontent.com/121559414/212614438-98d7a0c2-08bc-4d45-8a75-55bbf1722fb6.png)


JK FLIP-FLOP:

![q3](https://user-images.githubusercontent.com/121559414/212614488-de375ef0-a81d-4ecc-91a5-33657cdf846e.png)


T FLIP-FLOP:

![Q4](https://user-images.githubusercontent.com/121559414/212614563-54a98d8e-e9bc-4076-879d-3725990f5ac3.png)



RESULTS:

Thus, the program for flipflops is implemented and its functional table is successfully verified in quartus using Verilog programming.
