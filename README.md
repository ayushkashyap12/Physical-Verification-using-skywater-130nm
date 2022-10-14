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

   
     

    
     
