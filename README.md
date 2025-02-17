# LICexpt1

# Design circuit 1

# Aim : 

Perform DC Analysis, Transient Analysis and AC Analysis for the given circuit designs and get value of width of  such that power 50u .

# Components :

Mosfet (CMOSN) , resistors , DC power supply.

# Theory:

The common-source (CS) amplifier setup  is like the source is grounded, the gate receives the input signal, and the drain is connected to a resistor acting as the load. The transistor amplifies the input signal by modulating the drain current based on the gate-source voltage VGS. The drain resistor  RD converts the current variations into voltage changes, producing the amplified output signal.

**Operation:**

• Input Signal: The AC signal at the gate modulates the gate-source VGS , affecting the drain current Id.

• Amplification: The change in Id  causes a voltage drop across RD,producing an amplified output voltage at the drain.

• Voltage Gain: The voltage gain is given by: Av= -gm * RD.

where gm  is the transconductance of the MOSFET and RD is the drain resistor. The negative sign indicates signal inversion.
​
# Procedure :

**Part 1**

• Make the circuit connection.

• Connect resistor RD(1k ohm) to the drain of the mosfet , voltage source of 0.9V at gate of mosfet  and source of mosfet is grounded  .

• Apply voltage source of VDD(1.8V) to the resistor RD.

• Set length and width of mosfet as 180n and 1u .

• Perform DC analysis, Transient analysis and AC analysis by giving a sine wave to the voltage source at gate .

**Part 2**

• Consider power as 50u and calculate Id .

• Pick length of mosfet as 180n and vary width , till we get the calculated Id value .

• Perform DC analysis, Transient analysis and AC analysis by giving a sine wave to the voltage source at gate .


# Circuit 
 ![Screenshot 2025-02-17 191726](https://github.com/user-attachments/assets/75862588-acd5-4ba9-8b68-270e55f1201d)

# Observation

# Part 1
  ![Screenshot 2025-02-17 194428](https://github.com/user-attachments/assets/8f931ca7-6a6c-4f84-a9a8-319f6714711d)

**1) DC Analysis :**
  ** Procedure :**
   Select the dc output point(DC op pnt) in Simulation command and then Run.
   
   Below figure is what we get after DC analysis:
   
   ![Screenshot 2025-02-17 194454](https://github.com/user-attachments/assets/4c87c9ea-a6dc-43da-bd2c-8c25d7bf574c)

**2) Transient Analysis:**
 **  Procedure :**
   Select the Transient analysis in Simulation ,  Give the stop time as 5 ms and then Run.
   Put value of V2 voltage source at gate as sine wave of DC offset 0.9 v, amplitude as 50m and frequency 1k Hz.

    ** Graph**
    
![Screenshot 2025-02-17 194616](https://github.com/user-attachments/assets/a4a370be-9eb4-4520-8ac1-93773bfb3ea7)
   
**3) AC Analysis:**
   
** Procedure :**
 Select the ac analysis in configure analysis inside  Simulation ,with decade as type of sweep , number of points as 20 , start frequency 0.1Hz and stop frequency 1T Hz and then Run.

**Graph**
![Screenshot 2025-02-17 194730](https://github.com/user-attachments/assets/54adb390-1ee4-4eeb-a629-e148bc9c4c3e)


# Part 2
 # Calculation 
 
     Given , Power = 50u watts
     
              VDD= 1.8 V
           
     WKT,  Formula for power is 
     
                                    Power = Voltage * Current 
     
                                          P= VDD*Id
          
                                         Id= P / VDD

                           By substitution ,
          
                                          Id = 50u /1.8
          
                                       ** Id= 2.77*10^-5 A**


       ![Screenshot 2025-02-17 191739](https://github.com/user-attachments/assets/2c3a69d7-075f-44c5-acbd-33c0a8ae72ee)
   
**1) DC Analysis :**
   
** Procedure :**
   
    • Select the dc output point(DC op pnt) in Simulation command and then Run.
   
    • Below figure is what we get after DC analysis :
   
   ![Screenshot 2025-02-17 191715](https://github.com/user-attachments/assets/dba27530-8e1a-40fa-8e63-c2eea9b83c13)



**2) Transient Analysis:**
    
**   Procedure :**
   
•  Select the Transient analysis in Simulation ,  Give the stop time as 5 ms and thenRun.
   
 • Put value of V2 voltage source at gate as sine wave of DC offset 0.9 v, amplitude as 50m and frequency 1k Hz.;

  ** Graph **
  
      ![Screenshot 2025-02-17 193713](https://github.com/user-attachments/assets/d6f975f7-d04c-447c-b093-49f783f1c3c5)


   
**3) AC Analysis:**
   
  ** Procedure : **
   
•  Select the ac analysis in configure analysis inside  Simulation ,with decade as type of sweep , number of points as 20 , start frequency 0.1Hz and stop frequency 1T Hz and then Run.

 ![Screenshot 2025-02-17 194153](https://github.com/user-attachments/assets/d3c7b095-90ff-41e4-a830-077f00844bcc)

# RESULT( Design-1):

1) DC Analysis:

The DC analysis was performed by selecting the DC operating point. After running the simulation, we observed the DC operating point for the MOSFET. The result shows the drain current and voltage levels, confirming that the transistor is operating in the active region.

 2)Transient Analysis:
 
     A sine wave with a DC offset of 0.9V, amplitude of 50mV, and frequency of 1kHz was applied at the gate. The output voltage was observed at the drain, showing the amplified version of the input signal with signal inversion.

3) AC Analysis:
   
In the AC analysis, the frequency sweep was configured from 0.1Hz to 1THz, with 20 points in a decade sweep. This analysis shows the frequency response of the amplifier.

# Inference  ( Design-1):
   
  •  The DC analysis helps to set the biasing conditions for the MOSFET, ensuring that it is in the correct operating region (saturation) for amplification.
    
 •  The transient analysis shows how the input signal (AC) is amplified by the common-source configuration. The output signal exhibits amplification and inversion, which is characteristic of the common-source amplifier.

  •  The AC analysis provides insight into the frequency characteristics of the amplifier. It helps us observe the bandwidth and gain characteristics over a wide frequency range. This is important for understanding the amplifier's performance in different applications.


# Design Circuit 2
# Aim : 

Perform DC Analysis, Transient Analysis and AC Analysis for the given circuit with both nmos and pmos .

# Components :

Mosfets (CMOSN and CMOSP) , DC power supply.

# Theory:

The Common-Source (CS) Amplifier with a Current Source Load is a circuit where the MOSFET's (M1) load is replaced by a current source (M2) instead of a passive resistor. This modification greatly enhances the amplifier's performance, especially in terms of gain and operating range. It is widely used in integrated circuits due to its ability to deliver higher gain and improved performance compared to the traditional resistor-loaded CS amplifier.

 • Amplification Mechanism : The input signal modulates the gate-source voltage (Vgs) of M1, controlling the drain current (Id), which is mirrored by the current source (M2), providing high output impedance and increasing gain.

• Large-Signal Behavior: The output signal is an amplified version of the input, influenced by the transistors' nonlinearities.

• Small-Signal Behavior: The gain depends on M1’s transconductance (gm) and the parallel combination of output resistances (ro) of M1 and M2:
  
  Av = -gm * (ro_n || ro_p)
  
• Gain: The current source load provides higher gain due to the higher output resistance of M2 compared to a resistor-loaded amplifier.



# Procedure :

• Make the circuit connection.

• Consider a CMOSN mosfet.

• Connect CMOSP to the drain of the CMOSN , voltage source of 0.9V at gate of CMOSN and source of CMOSN is grounded  .

• Apply voltage source of VDD(1.8V) to the CMOSP.

• Set length and width of  CMOSN same as the previous circuit .

• Pick length of CMOSP as 180n and vary width , till we get the calculated Id value same as the privious circuit  .

• Perform DC analysis, Transient analysis and AC analysis by giving a sine wave to the voltage source at gate .

• Find V2

            | Vg - Vs| > |Vt|

          | Vg - 1.77| > | -0.366|

               | Vg | >  |1.38|


  # Circute 
  
![Screenshot 2025-02-17 224656](https://github.com/user-attachments/assets/d07f8a1b-dd58-479c-9296-6319c9ebe882)

# Observation 

![Screenshot 2025-02-17 230314](https://github.com/user-attachments/assets/b0b0ada7-daf6-49a8-b673-2e7bf51c2f93)

**1) DC Analysis :**

 **  Procedure :**
 
   Select the dc output point(DC op pnt) in Simulation command and then Run.
   
   Below figure is what we get after DC analysis
   
   ![Screenshot 2025-02-17 230242](https://github.com/user-attachments/assets/75143367-485e-4c04-900b-ae7b1afdfcfd)

  

**2) Transient Analysis:**

  ** Procedure :**
  
   Select the Transient analysis in Simulation ,  Give the stop time as 5 ms and thenRun.
   
   Put value of V2 voltage source at gate as sine wave of DC offset 0.9 v, amplitude as 50m and frequency 1k Hz.

   **  Graph**
   
    ![Screenshot 2025-02-17 224951](https://github.com/user-attachments/assets/246c5d28-befa-4ed0-9554-dacde703d635)


   
**3) AC Analysis:**
   
**   Procedure :**
 Select the ac analysis in configure analysis inside  Simulation ,with decade as type of sweep , number of points as 20 , start frequency 0.1Hz and stop frequency 1T Hz and then Run.

 ** Graph**
![Screenshot 2025-02-17 231611](https://github.com/user-attachments/assets/d06643a6-2708-4c38-86c0-5ff25469b1d4)

# RESULT( Design-2):
1) DC Analysis : The DC analysis validates the correct biasing of the MOSFETs, with the drain and gate voltages corresponding to the expected operating conditions.

2) Transient Analysis : The output signal at the drain amplifies the input sine wave, confirming the amplification process is functioning properly.

3) AC Analysis : The AC analysis illustrates the amplifier's frequency response, showing its gain and bandwidth characteristics across a wide frequency spectrum.



# Inference  ( Design-2):
   
The DC analysis verifies that the circuit is properly biased, with the transistor operating in the saturation region. The output accurately follows the input, showing amplification along with some distortion due to the MOSFET's nonlinear behavior. The signal stays within the expected range, and the circuit performs well with dynamic input signals. The gain remains stable across the frequency range, suggesting the amplifier operates effectively within the intended bandwidth. While high-frequency performance may be affected by the MOSFETs' intrinsic capacitances, the overall performance is strong.

