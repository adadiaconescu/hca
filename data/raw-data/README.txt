====
HCA: 
====

3 levels, identified as: 

-- L0 (bottom), 

-- L1 (middle), 

-- L2 (top).


34 CA, identified as:

-- A0 (the CA situated at L2; its raw-data file is L2A0.txt)

-- A1 (the CA situated at L1; its raw-data file is L1A1.txt)

-- A2..A33 (the CA situated at L0) 


E.g. raw-data files for CA at L0

-- Corner CA: L0A2.txt

-- Border CA: L0A3.txt

-- Core CA: L0A11.txt

The above files are used, as representatives of the three groups, to analyse behaviour at L0 (cf. *.xlsx files)




=========================================
Legend for files named _L<level no.>_all:
=========================================

level diversity count: the number of different states produced by all CA at this level, together. 


=================================================
Legend for files named _L<level no.>_A<CA index>:
=================================================

E.g. file L0A2.txt contains data from the CA2 (Corner) situated in L0.

LevelCount: index of simulation cycles (each cycles inclues the sequential activation of all HCA levels); 

AutomataStep: index of CA activation (for a 3-level HCA, this will be a third of the LevelCount); 

AggregateState: the aggregate state (0 or 1) sent to the supra-CA cell to which this CA is mapped;

Goal: the goal (0 or 1) from the supra-CA cell to which this CA is mapped. This CA reacts to goals by changing its rules;

StateDifference: the number of cells that have changed from the previous state and the current state;

DiversityCounter: the number of different states produced by this CA

LiveCellsCount: the number of live cells of this CA

LiveCellsArea: the CA's board area within which there are live cells 

LiveCellsDensity: the LiveCellsCount divided by the LiveCellArea

StateId: the state id for this CA's state (used to determine diversity count by comparison with previous states).



