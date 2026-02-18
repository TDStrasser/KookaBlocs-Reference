Glossary of Terms
=================

This glossary contains the definitions of terms used throughout this KookaBlocs Reference Guide 
and is intended to demystify the vocabulary often used in association with computers and software.


.. glossary::

    Kookaberry
      The **Kookaberry** is a microcomputer specifically designed for **STEM** educational applications.  
      See https://learn.auststem.com.au/exploring-the-kookaberry/

    KookaBlocs
      **KookaBlocs** is a visual code editor based on Google Blockly and is designed as a Progressive Web Application (PWA).
      **KookaBlocs** incorporates Google Blockly, an open-source developer library created by Google that provides a visual programming interface which 
      enables users to create programs by dragging and dropping interlocking, graphical blocks that represent code concepts.
      **KookaBlocs** is intended to be run on hardware using the Kooka Firmware such as a Kookaberry from Kookaberry Pty Ltd and Pico, 
      Pico 2 modules from Raspberry Pi.  Key characteristics of **KookaBlocs** include **Visual Programming** using a drag-and-drop interface with 
      puzzle-piece-like blocks, eliminating the need for users to write code line by line or worry about syntax.
      **KookaBlocs** can be launched using https://auststem.com.au/KookaBlocs/ 
      
    KookaCode
      **KookaCode** is a **MicroPython** scripting code editor and is designed as a Progressive Web Application (PWA). 
      **KookaCode** is intended to be run on hardware using the Kooka Firmware such as a Kookaberry from Kookaberry Pty Ltd 
      and Pico, Pico 2 modules from Raspberry Pi.
      **KookaCode** can be launched using https://auststem.com.au/KookaCode/

    KookaSuite (now deprecated)
      A suite of programming tools for the **Kookaberry** comprising **KookaBlockly** visual coding tool,
      **KookaIDE** a **MicroPython** integrated development tool, and **KookaTW** a tool for mirroring / virtualising the **Kookaberry**'s 
      display and buttons. Please note that **KookaSuite** has now been deprecated and will no longer be developed.
      KookaSuite has been replaced by **KookaBlocs** and **KookaCode**.
    
    Progressive Web Application (PWA)
      A PWA is a website that works and feels like a native mobile or desktop app, without needing to be downloaded from an app store.
      **KookaBlocs** and **KookaCode** are PWAs.
      Instead of opening **KookaBlocs** in a browser tab every time, you can install it once from the website. 
      It then appears on your home screen, taskbar, or app menu—just like a regular app.
      PWAs will work offline. They can cache content so they continue to work even if your internet connection drops or is slow. 
      When you go back online, they synchronise any changes.
      The developer can update a PWA instantly on their server, and everyone gets the latest version automatically. 
      By refreshing the browser while online, the latest updates will be automatically downloaded.
      See https://en.wikipedia.org/wiki/Progressive_web_app.


    Visual Programming
      Using a visual code editor (such as **KookaBlocs**) allows users to work with code visually but still involves actual code blocks or snippets. 
      It might use drag-and-drop interfaces, code blocks, or other visual elements to assist in code creation.
      Visual code editors often aim to make coding more accessible to beginners or those who are not familiar with traditional text-based coding environments.
      It differs from a graphical code editor that may involve more abstract graphical representations of code structures, while
      visual code editors usually retain a connection to the actual code, using visual elements to enhance the coding experience. 
      See also https://en.wikipedia.org/wiki/Visual_programming_language

    OLED
      Organic Light Emitting Diode - the lighting technology that is used in the **Kookaberry**'s display - see https://en.wikipedia.org/wiki/OLED

    LED
      Light Emitting Diode - a semiconductor that emits a specific wavelength of light when energised.  
      The **Kookaberry** has three LEDs on the front under the display. They emit red, yellow and green light.
      There are two further LEDs on the back: a green LED indicating the **Kookaberry** has power, 
      and a blue LED which indicates file writing activity, or if pulsing slowly indicates the **Kookaberry**'s power supply voltage is low.
      See also: https://en.wikipedia.org/wiki/Light-emitting_diode

    GPIO
      General Purpose Input and Output - the electrical signals to and from a microcomputer are connected by these, 
      and are referred to as :doc:`pins` by **KookaBlocs**. See also https://en.wikipedia.org/wiki/General-purpose_input/output
 
    USB
      Universal Serial Bus - a communications and power connection used by the **Kookaberry** to communicate with the programming personal computer,
      and the receive power.  See also https://en.wikipedia.org/wiki/USB.

    MicroPython
      A variant of the computer programming language **Python** developed for use on micro-computers.  
      The **Kookaberry** is programmed using **MicroPython** and has a built-in compiler accessible through editors such as **KookaCode**, 
      **KookaIDE** and **Thonny**.
      **KookaBlocs**, and its predecessor **KookaBlockly**, automatically generate **MicroPython** code when the user assembles a script 
      from visual blocks.
      See also https://en.wikipedia.org/wiki/MicroPython

    Python
      A high-level computer programming language that was designed to be easy to use and easily comprehended.  
      It nonetheless is a very powerful language and is now favoured by educational institutions as the first-taught computer language.
      See also https://en.wikipedia.org/wiki/Python_(programming_language)

    IDE
      Integrated Development Environment - a software application that integrates code editing, testing and sometimes code debugging tools.  
      Examples relevant to **KookaBlockly** and the **Kookaberry** are **KookaCode**, **KookaIDE** and **Thonny**. 
      See also https://en.wikipedia.org/wiki/Integrated_development_environment

    STEM
      Science, Technology, Engineering and Mathematics - an umbrella term to group these disciplines in the context of education and career development.
      See also https://en.wikipedia.org/wiki/Science,_technology,_engineering,_and_mathematics
   
    Raspberry Pi Pico
      A microcomputer developed by the **Raspberry Pi Foundation** based on their **RP2040** and **RP2350** microprocessor chips.  
      The **RP2040** microprocessor chip is used in later hardware versions of the **Kookaberry**.
      See also https://en.wikipedia.org/wiki/Raspberry_Pi

    STM
      STMicroelectronics N.V. commonly referred to as ST or STMicro is a multinational corporation and technology company of French-Italian origin.
      **STM** microprocessors are used in the original hardware version of the **Kookaberry**.
      See https://en.wikipedia.org/wiki/STMicroelectronics and https://en.wikipedia.org/wiki/STM32

    Micro:Bit
      A microcomputer for **STEM** applications developed in the United Kingdom by the BBC (British Broadcasting Corporation).  
      It also is programmed using **MicroPython**, and has two official visual programming tools, being **Microsoft MakeCode**, and **Scratch**.
      The **Micro:Bit** differs from the **Kookaberry** in that it can contain only one program at a time, it has just two buttons and an 8x8 LED matrix display, 
      and it has no electrical sockets with which to connect peripherals, relying instead on using alligator clips or an expansion board.
      See also https://en.wikipedia.org/wiki/Micro_Bit and https://en.wikipedia.org/wiki/Scratch_(programming_language)
  
    Windows
      A personal computer operating system licensed by **Microsoft**.  **KookaSuite** will run on **Windows** V10 and later versions.
      See https://en.wikipedia.org/wiki/Microsoft_Windows

    MacOS
      A personal computer operating system developed by **Apple**.  
      **KookaSuite** will run on MacOS V13 and later versions using the **Intel** and **Apple**'s M processors.
      See also https://en.wikipedia.org/wiki/MacOS

    Raspbian
      Latterly named Raspberry Pi OS, a personal computer operating systems for the Raspberry Pi microcomputer licensed by the **Raspberry Pi Foundation**.  
      **Raspbian** is based on the **Debian Linux** operating system.
      See also https://en.wikipedia.org/wiki/Raspberry_Pi_OS

    Thonny
      An open-source Integrated Development Environment tool tailored for programming in **Python**. 
      See https://en.wikipedia.org/wiki/Thonny
      
    Firmware
      Low-level computer software that is stored on on-board non-volatile memory.  
      It performs basic low-level tasks to control and monitor the computer hardware, and to make it accessible to high-level software, such as **MicroPython**.
      **Firmware** updates may sometimes be issued that extend the functionality of a computer, or to remedy bugs or security weaknesses in the **firmware**.
      The **Kookaberry**'s **firmware** is updated from time to time for the same reasons.
      See also https://en.wikipedia.org/wiki/Firmware

    Real Time Clock (RTC)
      A specialised clock chip that keeps precise time.  **RTCs** can be built into a microcomputer and / or be connected externally.  
      Often external **RTCs** have a small battery that keeps the clock running when the microcomputer is turned off.  
      The microcomputer can then synchronise its internal **RTC** with the battery-powered external **RTC**.
      See also https://en.wikipedia.org/wiki/Real-time_clock

    ASCII
      American Standard Code for Information Interchange - a character encoding standard for electronic communication. 
      **ASCII** codes represent text in computers, telecommunications equipment, and other devices.
      **MicroPython** uses **ASCII** code when encoding character strings.
      See also https://en.wikipedia.org/wiki/ASCII
    
    CSV
      Comma-Separated-Values - a text file format in which each line contains alphanumeric text data which are separated by commas. 
      The first line of the files can be used to represent headings for the data item columns that are in the following lines.
      **CSV** formatted files are recognised and can be directly opened by spreadsheet programs.
      See also https://en.wikipedia.org/wiki/Comma-separated_values

    GitHub
      A software platform that allows developers to create, store, and manage their code. **GitHub** was acquired by **Microsoft** in 2018.
      It is commonly used to host **open-source** **software** development projects.
      **KookaSuite** and the **Kookaberry** **firmware** are both distributed using **GitHub**.
      This document is also maintained and distributed using **GitHub** and **Read the Docs**.
      See also https://en.wikipedia.org/wiki/GitHub 

    Read the Docs
      **Read the Docs** is an open-source free software documentation repository and hosting platform.  This document is hosted on Read the Docs.
      See also https://en.wikipedia.org/wiki/Read_the_Docs

    Open-Source
      Open source is **software** source code, **hardware** designs, documentation, artworks or other intellectual products that are made freely available 
      for possible modification and redistribution, under certain licensing conditions, in a spirit of sharing and collaboration for the greater good.
      See also https://en.wikipedia.org/wiki/Open_source

    Software and Hardware
      **Software** is a collection of programs and data that tell a computer how to perform specific tasks. 
      **Software** often includes associated **software documentation**. 
      This is in contrast to **hardware**, which comprises the physical components from which the system is built 
      and which actually performs the computing work.
      See also https://en.wikipedia.org/wiki/Software and https://en.wikipedia.org/wiki/Computer_hardware