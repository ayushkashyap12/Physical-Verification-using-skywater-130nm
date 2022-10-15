# Physical-Verification-using-skywater-130nm
Physical Verification using skywater 130nm

![background](https://user-images.githubusercontent.com/92054999/195906638-ccb690ca-5c2e-4972-8c3c-1e27d43d57c5.PNG)

## Brief Description of the Workshop
# *Index*

- [Physical Verification using skywater 130nm](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Physical-Verificatio-using-skywater-130nm)
    - [Brief Description of the Workshop](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Brief-Description-of-the-Workshop)
      -  [Day 1 -Physical Verification using skywater 130nm](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Physical-Verificatio-using-skywater-130nm)
          -  [Part 1:Introduction to open-source magic,xschem,netgen](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Part-1-Introduction-to-open-source-magic-xschem-netgen)
          -  [Part 2:Simulation using xschem](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Part-2-Simulation-using-xschem)
          -  [Part 3:Layout using Magic](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Part-3-Layout-using-Magic)
          -  [Part 4:LVS using netgen](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Part-4-LVS-using-netgen)
      
      -  [Day 2 -Introduction to DRC and LVS](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Introduction-to-DRC-and-LVS)
           -  [Part 1- GDS Read](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Part-1-GDS-Read)
           -  [Part 2- PORTS](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Part-2-PORTS)
           -  [Part 3- ABSTRACT VIEW](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Part-3-ABSTRACT-VIEW)
           -  [Part 4- BASIC EXTRACTION](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Part-4-BASIC-EXTRACTION)
           -  [Part 5-SETUP FOR DRC](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Part-5-SETUP-FOR-DRC)
           -  [Part 6-SETUP FOR LVS](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Part-6-SETUP-FOR-LVS)
      
      -  [Day 3 -Design rule check ](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Day-3-Design-rule-check)
      
           - [Part 1- Fabrication process](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Part-1-Fabrication-process)
           - [Part 2- DEVICE RULE](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Part-2-DEVICE-RULE)
           - [Part 3- LATCH UP RULE](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Part-3-LATCH-UP-RULE)
           - [Part 4- DENSITY RULE CHECK](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Part-4-DENSITY-RULE-CHECK)
      
        -  [Day 5 -LAYOUT VERSUS SCHEMATIC ](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Day-5-LAYOUT-VERSUS-SCHEMATIC)
      
           - [Part 1- Part 1- Installation](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Part-1-Installation)
           - [Part 2- Introduction-Fundamentals of LVS](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Part-2-Introduction-Fundamentals-of-LVS)
           - [Part 3-LVS with subcircuits and blackboxes](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Part-3-LVS-with-subcircuits-and-blackboxes)
           - [Part 4-LVS with Analog block](https://github.com/ayushkashyap12/Physical-Verification-using-skywater-130nm/edit/main/README.md#Part-4-LVS-with-Analog-block)
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
      
    # Day 1: Introduction of the open source tool and Installation
    
    On the first day,we learnt about the open source tool i.e magic,xschem,netgen and its uses , simulation of cmos Invertor was done using xschem and the simulation was verified.
    
    ## Part 1:Introduction to open-source magic,xschem,netgen
     First, we created the folder of the each tool using mkdir and then linking folder to pdk  i.e skywater pdk
      ![l1_intro](https://user-images.githubusercontent.com/92054999/195911776-3ae6610e-ea51-4ada-b2ed-c3627c744726.PNG)
     
     
     Linking from pdk was done using the command ln -s as shown below:
      ![l2](https://user-images.githubusercontent.com/92054999/195911999-78927434-40c9-46a6-aea3-2c5ffb276175.PNG)
      
    ## Part 2:Simulation using xschem 

     The homepage of the xschem is shown below, which explains about the various device details of the pdk
      ![xchem_home](https://user-images.githubusercontent.com/92054999/195915488-e816a23a-59ed-4acc-882c-702f82063b7a.PNG)

     Simple circuit i.e cmos Invertor was taken to explain the use of xschem.The nmos and pmos was taken from the sky130_fd_pr as shown below:
      ![l3_xschem](https://user-images.githubusercontent.com/92054999/195914073-f55e9c29-3427-4af0-9d30-a2973c88a17f.PNG)
      
     The schematic figure was made by setting the correct nmos and pmos parameter.
      ![l4_invertor](https://user-images.githubusercontent.com/92054999/195914297-bf7fa0e2-ef5f-489f-94da-7352539ce8c5.PNG)
    
     To test the  schematic,test circuit was made by giving the proper input to have correct transfer characteristics.
      ![d5](https://user-images.githubusercontent.com/92054999/195914658-8f91c03b-9ea1-4312-bffc-d4074abdd648.PNG)

     The transfer characteristics obtained of the above cmos Invertor using xschem is shown below:
      ![simulation_result](https://user-images.githubusercontent.com/92054999/195915285-b1af5218-dcda-4470-87ed-313380d4585b.PNG)
      
    ## Part 3:Layout using Magic
     Magic - Upon properly setting up, we can find the technology used as SKY130 to look in a better 3D view use  magic -d XR  and magic -d OGL - for  Faster.
     The home page of the magic is shown below, I have created the folder mag in the proj file and opened using the command 'magic'
     ![magic_open](https://user-images.githubusercontent.com/92054999/195916903-32fc283c-4781-4196-acfc-6e78398e1e08.PNG)
     
     The Nfet layout was taken into example to explain the layout and the wiring.
     ![magic1](https://user-images.githubusercontent.com/92054999/195917816-4b9570a3-7e1e-4da7-b59c-a004e5f2a91f.PNG)

     Cmos Invertor was made using this tool as shown below:
     ![magic2](https://user-images.githubusercontent.com/92054999/195917964-4cb90314-ee9b-43ad-852a-10aad69c3340.PNG)
     ```
     Perform extraction using-
      extract do local
      extract all
      ext2spcie lvs
      ext2spice
      quit
      
     ```
   ngspice - Used to study the various behavioour of the design made. Plot functions based on various criteria is readily available.


   ## Part 4:LVS using netgen 
   netgen - LVS utility that checks the LVS(layout versus schematic) between netlists to verify geometry.
   The basic example was taken to explain the use of this tool.
   ![D5_l2_result_lvs](https://user-images.githubusercontent.com/92054999/195919690-6c05e7a1-73c7-4c2f-8fcc-a0374966ece3.PNG)

  #  Day 2 -Introduction to DRC and LVS
   ## Part 1- GDS Read
    The following code was used to read the gds file:
    ```
    mkdir lab_2
   cd lab_2
   mkdir mag
   cd mag
   cp /usr/share/pdk/sky130A/libs.tech/magic/sky130A.magicrc ./.magicrc
   magic -d XR
   ```
   ![D2_L1](https://user-images.githubusercontent.com/92054999/195922788-d0e87174-89d4-4aed-bb26-97dab84b36b4.PNG)
   After the console
   ![d2_l2](https://user-images.githubusercontent.com/92054999/195923497-380b3870-db4c-4e4f-a065-87cb620a97d0.PNG)
   Go to options-->cell manager --> Top down list and select aky130_fd_sc_hd_and2_1 i.e two input and gate to analyze the layout.
   ![d2_l3](https://user-images.githubusercontent.com/92054999/195924393-22509331-49d1-4154-bc61-ef5ce4a3d40b.PNG)
   
   ## Part 2- PORTS
    To see check ports in the layout.
   ![d2_l4_ports](https://user-images.githubusercontent.com/92054999/195925779-196adffe-db55-4b67-a9a4-74533baa03b2.PNG)
   ## Part 3- ABSTRACT VIEW
    The abstract view can be seen in magic tool

   ![d2_l7_abstract](https://user-images.githubusercontent.com/92054999/195926940-976c2a88-4aff-44f1-aca6-d1c0737b819b.PNG)
   ## Part 4- BASIC EXTRACTION
    The code shown below was used:
    ```
    magic -d XR
    load sky130_fd_sc_hd__and2_1
    extract all
    ext2spice lvs
    ext2spice
    ext2spice cthresh 0
    ext2spice

    ```
    The result obtained is shown below:
    ![d2_I8_extraction](https://user-images.githubusercontent.com/92054999/195927407-181e30b1-91a6-47c5-b938-ecd213d40518.PNG)
 
    
   ## Part 5-SETUP FOR DRC
    The  below code was used
   ```
   /usr/share/pdk/sky130A/libs.tech/magic/run_standard_drc.py /usr/share/pdk/sky130A/libs.ref/sky130_fd_sc_hd/mag/sky130_fd_sc_hd__and2_1.mag
   magic -d XR
  load sky130_fd_sc_hd__and2_1
  
  ```
   ![d2_I8_DRC](https://user-images.githubusercontent.com/92054999/195927786-5f407cfa-0996-4a75-84a0-e04b91569fd5.PNG)
   
   ## Part 6-SETUP FOR LVS
     The  below code was used
   ```
   mkdir netgen 
   cd netgen
   cp /usr/share/pdk/sky130A/libs.tech/netgen/sky130A_setup.tcl ./setup.tcl
   cd ../mag
   magic -d XR sky130_fd_sc_hd__and2_1
   
   ```
   The results of LVS is shown below:
   ![d2_I8_lvs](https://user-images.githubusercontent.com/92054999/195928388-48d2a08e-d638-40d6-a742-3957f5d86722.PNG)
 
   ![d2_lvs result](https://user-images.githubusercontent.com/92054999/195928450-9a0c14a4-1ef1-4318-a273-6e47fbeedc7a.PNG)
   
   # Day 3 -Design rule check
   on the third day , the fabrication process was studied and detailed study about design rule check(DRC) was analyzed.
   
    ## Part 1- Fabrication process
      Silicon manufacturing process is mostly  a planar process and the layers are added onto or implanted into other layers.
      Masks - These are placed on our various layers and the photoresist is broken down. Now the ion implantation or acid etching can be carried out through the space created.
    ![u1](https://user-images.githubusercontent.com/92054999/195971303-9c17ef33-292b-45c9-9c9b-984b72703064.PNG)
    
    As the spacing is reduced the probability of failure increases exponentially!

    DRC is all about  minimum spacing to get a good process yield, if we space it wider than that, the process yield gets better, but more space is consumed and depends on what we want .

    The link of  DRC documentation of Skywater PDK is given below -

    https://skywater-pdk--136.org.readthedocs.build/en/136/rules.html
    
    ![u2](https://user-images.githubusercontent.com/92054999/195971738-8467c4ce-90d9-4496-b84c-2865560516b0.PNG)

    ## Part 2- Metal Layer rule
     The file from the pdk was Installed at the specific folder,which is mentioned below:
       ![d3_l1_cloning](https://user-images.githubusercontent.com/92054999/195972090-f9a2a739-45ca-46ab-9750-24634da562c7.PN

     Wide-spacing rule
      If one piece of the structure is wider than a given width, other wires of any width must be spaced apart at a greater distance.
      Basically, Metals >3 microns trigger widespacing rule in SKY130.
      Below figure is attached to explain the metal spacing rule.
      ![d3_l3_drc](https://user-images.githubusercontent.com/92054999/195973308-a5027092-1330-4271-aa73-67d4c4969c1c.PNG)

     Notch rule
       Notch rule is associated with a fork geometry.The notch rule snippet is attached below:
        ![d3_l5](https://user-images.githubusercontent.com/92054999/195973372-9bb20a6c-acf7-4fac-855b-4e5cd2d0608f.PNG)
        ![d3_l2_drc](https://user-images.githubusercontent.com/92054999/195972794-d0192bbd-3591-43e1-a63a-2d1b6e876d59.PNG)
      Minimum and maximum area rules
       It Gives the minimum and maximum areas for a metal layer and the below snippet shows the same.
        ![d3_l9](https://user-images.githubusercontent.com/92054999/195973450-63db2c12-b096-439c-aec3-a819e07e9893.PNG)
        
     ## Part 2- DEVICE RULE
     
        Resistors
         Resistors can be made out of diffusion layers, polysilicon layers or p-well regions deep inside n-wells.
         
        Capacitors
         There are different types i.e Varactor, MOSCAP, MiM and Vertical Parallel plate (VPP) or MoM.  MiM is mostly used and  has a very high capacitance.
          Note:Aspect ratio regulations, bottom and top layer regulations, and antenna regulations are all applicable to MiMs.
          
        Diodes
         Diodes can be formed by a well and a diffusion layer.
         ![d3_I10](https://user-images.githubusercontent.com/92054999/195974863-91b690d0-103a-4f19-8c61-c9c110c1560b.PNG)
         
     ## Part 3- LATCH UP RULE
     Latch-up rules :due to parasitic bipolar transistor formed between taps, wells and substrate - the rules will generate minim distance between tap connection and                        any diffusion zone.
         ![d3_i12_latchup](https://user-images.githubusercontent.com/92054999/195979446-210342cf-a096-456d-99b7-71b4e63fde25.PNG)

     ## Part 4- DENSITY RULE CHECK
     To reduce bumpiness of the surface after oxide growth and polishing, we place metal layers and in between them add some 'fill metals', so the surface after polishing is evenly smooth.
         ![d3_I14_density](https://user-images.githubusercontent.com/92054999/195979486-a1562c0e-8cb2-4c93-ae1d-a0ea37513296.PNG) 
         ![d3_I13_densityres](https://user-images.githubusercontent.com/92054999/195979498-9c9188a5-2871-4d74-8c2f-8064a2a5467b.PNG)
        
    #  Day 5: LAYOUT VERSUS SCHEMATIC
     On the last day, we analyzed about the LVS step,which is followed before tapeout to verify the circuit.
      
     ## Part 1- Installation
      To verify the LVS , we have installed the PDK to a specified folder.
         ![d5_l1_starting_gitclone](https://user-images.githubusercontent.com/92054999/195980403-13293ee1-83ff-47cd-bb0a-77aa25eca79e.PNG)
         
     ## Part 2- Introduction-Fundamentals of LVS
      The designer does both LVS and DRC before tapeout and the netlists produced by each of the processes is compared with each other and matched. After tapeout,     its  send to the foundry, where it does DRC again before final processes.
      Basically , LVS is done by comaring the schematic netlist and the layout netlist.Opensource tool i.e. netgen is for doing LVS and can understand ssimulatable formats like VerilogRTL and SPICE. Schematics are made in Xschem with the components.

      
       The following results were obtained:
          ![D5_l2_result_lvs](https://user-images.githubusercontent.com/92054999/195981288-76b6ad57-a42e-4f38-827a-f123c73fef3a.PNG)
           
     ## Part 3-LVS with subcircuits and blackboxes
      To overcome writing lengthy command every time, we can actually create a bash script for the same
          ![d5_l3_subckt](https://user-images.githubusercontent.com/92054999/195981312-9e2ade40-d417-4014-9605-4dedc1cacd03.PNG)
          ![d5_l5_splowlevel](https://user-images.githubusercontent.com/92054999/195981524-3099d2eb-9568-4271-947d-cc2647353c44.PNG)
                
     ## Part 4-LVS with Analog block
      Power-On Reset- Every time power is applied to a certain electrical device, a power-on-reset circuit generates resetting signals.By doing so, you can           identify a known state in which the device always turns on or activates.
          ![d5_l11_analog](https://user-images.githubusercontent.com/92054999/195986957-da03ca81-cc5d-46f7-b233-be488fc20f38.PNG)
       The block on which LVS is being performed i.e. small analog block
          ![d5_l12](https://user-images.githubusercontent.com/92054999/195986966-37eef5e7-7dfc-4d53-9df1-b60a71b05edb.PNG)
