



#  REQUIREMENTS


# LOW LEVEL REQUIREMENTS

# Software used :

# SimulIDE  : 

     SimulIDE is a simple real time electronic circuit simulator which is open source.
     
     It is not so much professsional but it is very easy to use and have enough features to learn and do projects with microcontrollers like
          
          PIC , AVR and ARDUINO BOARDS.
          
# Features:

     Analog and Digital components.
     Microcontrollers.
     Code Editor.
     Debugger.
     Subcircuits.
     DIP/Logic Symbols.
     Circuit Animation.
     Basic Shapes.
     Oscilloscope.
     Signal Plotter
     Serial Port Connection.
     Serial Monitor.


# HIGH LEVEL REQUIREMENTS

 COMPONENTS USED IN THIS REMINDER PROJECT :
     
      AVR MICROCONTROLLER - Atmega328
      LEDS - 8
      Relay - 1 
      Buzzer - 1
      External supply - 5V (To turn on Relay)
      Pulse Width Modulation (PMW) Technique
      SimulIDE Software
      

# SWOT Analysis

STRENGTH : Anti theft protection , security and used as an alarm.

WEAKNESS : Just an intimation if anything happens .

OPPURTUNITY : Increase the security.

THREAT : lot of versions are already build.



# 4W'S

Where: It can be developed in home as well as security point of view.

When : Anytime and anywhere .

Who : People who needs protection and security as well as reminder.

Why : It is a easy use of method .

# 1H'S

How : when relay gets triggered the 8 leds glowing with an intimating buzzer sound.



# Bill of Materials:


atmega328-1 : atmega328

RelaySPST-7 : RelaySPST  

AudioOut-9 : AudioOut   

Led-10 : Led   
Led-11 : Led   
Led-12 : Led   
Led-13 : Led   
Led-14 : Led   
Led-17 : Led   
Led-18 : Led   
Led-20 : Led   
 

# Block Diagram

![Screenshot (13)](https://user-images.githubusercontent.com/94359739/144398422-31fc4577-b30b-4e73-a559-131f9ae7c890.png


# Source code 

#define F_CPU 16000000
#include <avr/io.h>
#include <util/delay.h>
int main(void)
{
	DDRB=0xFF;
	unsigned char z;
	while(1)
	{
		
		for(z=0;z<255;z++)
		{
			PORTB=z;
			_delay_ms(1000);
		}
	}
	return 0;
	}

      
        

     
