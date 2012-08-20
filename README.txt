README file for SEGY-formatted files which accompany paper:  
“Benchmark hydrogeophysical data from a physical seismic model” 
by Juan M. Lorenzo, David E. Smolkin, Christopher White, 
Shannon R. Chollett and Ting Sun published in "Computers
and Geosciences".
  

Eight files, numbered WL1.sgy through WL8.sgy, contain seismic 
data collected whenat eight different water levesl in the 
Sand Tank.

Each SEG-Y formatted file (Barry  ) consists of an initial 
3200-byte tape header (in EBCDIC format), followed by a 400-byte 
binary tape header, and 64 contiguous sets of data streams, or traces, 
one for each sensor in the arrray. Each trace is of equal length 
(standard SEG-Y format) and also contains a 240-byte binary header 
followed by 780 amplitude values recorded in a 4-byte IBM floating point format.  
These binary headers store metadata for traces as one or 
two-byte integers values.  Key information includes the sampling 
interval of 13 microseconds, and the number of samples: 780.

Each trace represents data collected at an accelerometer within a 
composite shot gather. Source-receiver offsets range from 0.03 -.87 m but 
the source-receiver values are not included in the headers.

SEGY data can be viewed in several open source software, such as Seismic 
Unix from the ColoradoSchool of Mines, Center for Wave Phenomena 
(www.cwp.mines.edu). 

References
Barry, K.M., Cavers, D.A., Kneale, C.W., 1975. Report on recommended 
standards for digital tape formats. Geophysics 40, 344-352
