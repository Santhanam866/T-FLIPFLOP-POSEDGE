# T-FLIPFLOP-POSEDGE

**AIM:**

To implement  T flipflop using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**T Flip-Flop**

T flip-flop is the simplified version of JK flip-flop. It is obtained by connecting the same input ‘T’ to both inputs of JK flip-flop. It operates with only positive clock transitions or negative clock transitions. The circuit diagram of T flip-flop is shown in the following figure.

![image](https://github.com/naavaneetha/T-FLIPFLOP-POSEDGE/assets/154305477/458a68fe-2d08-4a9d-ac4f-7ae0480ce0bd)

 
This circuit has single input T and two outputs Qtt & Qtt’. The operation of T flip-flop is same as that of JK flip-flop. Here, we considered the inputs of JK flip-flop as J = T and K = T in order to utilize the modified JK flip-flop for 2 combinations of inputs. So, we eliminated the other two combinations of J & K, for which those two values are complement to each other in T flip-flop. The following table shows the state table of T flip-flop.

Here, Qtt & Qt+1t+1 are present state & next state respectively. So, T flip-flop can be used for one of these two functions such as Hold, & Complement of present state based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of T flip-flop. Inputs Present State Next State

![image](https://github.com/naavaneetha/T-FLIPFLOP-POSEDGE/assets/154305477/cdd7fb32-539f-4b66-bb8d-f305a153c886)

 
From the above characteristic table, we can directly write the next state equation as Q(t+1)=T′Q(t)+TQ(t)′ ⇒Q(t+1)=T⊕Q(t)

**Procedure**

/* write all the steps invloved */


*Type the program in Quartus software.

*Compile and run the program.

*Generate the RTL schematic and save the logic diagram.

*Create nodes for inputs and outputs to generate the timing diagram.

*For different input combinations generate the timing diagram.

**PROGRAM**

/* Program for flipflops and verify its truth table in quartus using Verilog programming. 

module exp9(t, clk, rst, q);  


  input t, clk, rst;

  
  output reg q;

  

  always @(posedge clk or posedge rst) 

  
begin


    if (rst)

    
      q <= 0; 

      
    else if (t==0)

    
      q <= q; 

      
     else

     
        q<=~q;

        
  end

  
endmodule




Developed by:SANTHANAM S

RegisterNumber:24900166
*/2

**RTL LOGIC FOR FLIPFLOPS**
![388106874-8b134136-29d1-4547-b20e-1620a03e4f91](https://github.com/user-attachments/assets/12af99eb-1062-4ca0-bee5-9cc80838d4f3)

**TIMING DIGRAMS FOR FLIP FLOPS**
![388106939-0446cc37-2c18-4513-aa1d-a3785d948625](https://github.com/user-attachments/assets/9ab47d3a-8c2e-4513-82b0-41f0d8f83513)

**RESULTS**

To implement T flipflop using verilog and validating their functionality using their functional tables has been successfully completed.
