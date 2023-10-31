Compilacion Main MKS Robin Nano v1.3 con TFT35v1

Version BP = Bucket Purge  --> tiene ampliado el margen de X en 30mm para realizar la purga cambio material fuera de la cama.


Opciones habilitadas:


PID cama / Hotend. calibracion actualizada. 
	*Ideal que realicen la prueba y validen su calibracion. 
	*conectar a Pronterface y enviar comando 
	*M303 E0 S210 C8 --> pra Hotend 
	*M303 E-1 S70 C8  --> para cama 

	*grabar resultados con M301 para hotend y M304 para Cama 

Jerk
	* Default Jerk limits (mm/s)
	* Override with M205 X Y Z . . . E
	*
 	* "Jerk" specifies the minimum speed change that requires acceleration.
 	* When changing speed and direction, if the difference is less than the
 	* value set here, it may happen instantaneously.

S-Curve Acceleration
 	*
 	* This option eliminates vibration during printing by fitting a Bézier
 	* curve to move acceleration, producing much smoother direction changes.
 	*
 	* See https://github.com/synthetos/TinyG/wiki/Jerk-Controlled-Motion-Explained

XY Frequency limit
 	* Reduce resonance by limiting the frequency of small zigzag infill moves.
 	* See https://hydraraptor.blogspot.com/2010/12/frequency-limit.html
 	* Use M201 F<freq> G<min%> to change limits at runtime.

Adaptive Step Smoothing : 
	*increases the resolution of multi-axis moves, particularly at step frequencies
 	* below 1kHz (for AVR) or 10kHz (for ARM), where aliasing between axes in multi-axis moves causes audible
 	* vibration and surface artifacts. The algorithm adapts to provide the best possible step smoothing at the
 	* lowest stepping frequencies.

Power Loss recovery

	* Store the current state to the SD Card at the start of each layer
   	* during SD printing. If the recovery file is found at boot time, present
   	* an option on the LCD screen to continue the print from the last-known
   	* point in the file.

 Lin Advance ó  Linear Pressure Control v1.5
 	* Con Scurve y Low ejerks activado 
	* Assumption: advance [steps] = k * (delta velocity [steps/s])
	* K=0 means advance disabled.
 	*
 	* NOTE: K values for LIN_ADVANCE 1.5 differ from earlier versions!
 	*
 	* Set K around 0.22 for 3mm PLA Direct Drive with ~6.5cm between the drive gear and heatbreak.
 	* Larger K values will be needed for flexible filament and greater distances.
 	* If this algorithm produces a higher speed offset than the extruder can handle (compared to E jerk)
 	* print acceleration will be reduced during the affected moves to keep within the limit.
 	*
 	* See https://marlinfw.org/docs/features/lin_advance.html for full instructions.

Print Counter 
	*estadisticas de trabajos en el equipo. 

Eeprom 
	* permite almacenar en eprom desde menu pantalla 


