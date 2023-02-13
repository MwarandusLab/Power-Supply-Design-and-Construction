# Construction of Transformered Power Supply 

A transformed power supply is a device that converts high voltage, low current AC power from a wall outlet into low voltage, high current DC power that can be used to power electronic devices.

### Components Used
    1. Transformer having 12V and 2A Output Rating 
    2. Rectifier Diodes: I used 1N4007 having maximum voltage rating of 1000V AC and 1A
    3. Filter Capcitor: 3300uF 25V
                    **Equations Used**

        To find the value of C1 the following Equation will be used


                           5 x IO
                   C =  ------------
                           Vp x f

        Where; IO = Load Current
                     Vp= Peak Voltage
                      f = frequency and it is said to be twice the AC frequency (100Hz for 50Hz)
                      C = Capacitance in Farads
        Therefore;
                IO = 1A
                Vp = 12V (Output of transformer) x √2 =16.97V
                f = 100Hz

                 5 x 1 
        C =  -------------
              16.97 x 100

        C = 2.946 x 10-3 Farads
        C = 2946 Micro Farads

        Since there is no capacitor of that value then we should pick a capacitor of a closer value but greater than.
        I managed to get a 3300uf Electrolytic Capacitor, to determine the voltage rating of the capacitor to be used; Capacitor Voltage Rating > Vp (Peak Voltage).
        In my case i used 3300uf 25V Capacitor.

    4. Regulator: I went with the L7812 having maximum voltage rating of 35V DC and 1A 
    5. For the power code i used a flower cable to connect the primary wires of the transformer
    
## To construct a transformed power supply that supplies 12V and 1A, the following steps should be followed:

  1. Obtain all necessary components including a transformer, rectifier, filter capacitor, regulator and power cord.   

  2. Wire the transformer to the power cord to convert the high voltage AC power into low voltage AC power.

  3. Use the rectifier to convert the low voltage AC power into high voltage DC power.

  4. Connect a filter capacitor to the output of the rectifier to smooth out any fluctuations in the DC power.

  5. Use a voltage regulator to adjust the high voltage DC power to a stable 12V DC power with a maximum current of 1A.

  6. Connect the output of the voltage regulator to a terminal block to provide a convenient connection point for the electronic device.

  7. Test the transformed power supply to ensure it is supplying the correct voltage and current to the connected device.

  ## Block Diagram
  ![My Image](/Images/Block-diagram.png)
  
  ## Circuit Diagram
  ![My Circuit](/Images/Crcuit-diagram.png)
  
  ## Results
  ![My Results](/Images/Results.png)
  
  ## Conclusion
  Losses due to resistance of wire and temperature affects the semiconductor breakdown voltage which makes the expected value is not equal to practical value.
