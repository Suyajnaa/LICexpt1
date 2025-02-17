# LICexpt1

Aim : Perform DC Analysis, Transient Analysis and AC Analysis for the Given Circuit Designs and get value of width of  such that power 50u ;

Components : Mosfet (CMOSN),resistors,DC power supply.

Procedure :
Part 1
• Make the circuit connection.

• Connect resistor RD(1k ohm) to the drain of the mosfet , voltage source of 0.9V at gate of mosfet  and source of mosfet is grounded  .

• Apply voltage source of VDD(1.8V) to the resistor RD.

• Set length and width of mosfet as 180n and 1u .
• 



# Circute 

   ![Screenshot 2025-02-17 191726](https://github.com/user-attachments/assets/75862588-acd5-4ba9-8b68-270e55f1201d)

Using the Formula for Power, 

P=V*I

We will get the Values of Id as,

Id= 5.56 * 10^-5 A

we have to get the output current, Id for the given circuits by adjusting the values of L & W( Length and Width of the Channel of the MOSFET)

Length and Width of the Channel used to obtain the given Current is shown in the figure below;

   ![Screenshot 2025-02-16 120802](https://github.com/user-attachments/assets/109d353f-a954-4e08-b8d1-603ea40ea67c)

1) DC ANALYSIS:

   Procedure for Performing DC Analysis:
   we have to select the dc output print(DC op pnt) in the Edit Simulation Command and Run the Simulation

   ![Screenshot 2025-02-16 121422](https://github.com/user-attachments/assets/8dbd733e-f0a2-4165-8a8e-ebee3b28ace2)

   The Figure below shows the Values obtained from the DC Analysis : 

   ![Screenshot 2025-02-16 121045](https://github.com/user-attachments/assets/22bca609-a67e-4459-aa60-e584eb189442)

2) Transient Analysis:
