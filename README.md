# novaseq_training

## Library prep

300-500 range is the optimal size

600 cycle sequencing is only available on the MiSeq
On the NovaSeq the maximum can be 500 cycles on the S-prime

Clusters: group of DNA positioned closely together, each cluster represents thousands of copies of the same DNA strand in a 1-2 micron spot. The spot is about a micron. You need to have the dilution of thelibrary such that they can evenly space the single stranded DNA library

MiSeq is 1000 DNA stand cluster
Next seq is a 5000


Patterned Flow cell has a higher cluster density

Shut down the instrument from the software and then shut down the instrument from the switch.

How long do you keep the 1N NaOH before you consider it expired.
Use new bottles/smallest bottle possible.
1N NoOH solutions are not stable enough. Personally not keep it more than 6 months.

Frozen aliquots: Still thorw them out after 6 months.

Paired-end reading
When Illumina started, it could only do 36 bases and that was a knowledge to align them.
But when you have information about the both ends you have a better chance of good alignment.

## Index Reads
Index seq is a separate process
Another limitation of sequencing is longer you sequence, lower the quality of your sequence

Experiment Manager/Local Run Manager/Base Space/

You can use Base Space for run monitoring. Proactive us a component of Basespace.

## Index hopping 
Combinatorial Dual Indexes
Combinatorial Unique Dual Indexes


## Primary analysis
.bcl file are the primary data that comes out of the sequencer. Its one for every tile that is sequenced. 

*RTA2 and RTA3

## Image Analysis Overview RTA 1

RunInfo.xml, images and this will result in the data files.


Color normalization is done in the first 26 cycles

As we progress throught the cycles, the signals would drop. It used to compensate by amplifying the intensity. 
An example: there was a loss of signal and the machine was calling this as a G

Cluster location are .clocs
Cluster Intensities are .cif

Base calling and quality score are .bcl

Phasing needs to be <0.4%. This happens when a library in the cluster will have a base being read that is shorter on the sequence
Prephasing will be sequencing the read that is next to the majority of them being read.

These could happen alot with expired reagents. 
Could happen due to worng washing, tween 20 concentration/contamination
Do temporal lines washing. On Miseq do it once a month. Use bleach.

On four color chemistry, the base with the highest intensity is called.

*Pass filter*

IT measures the intenisty of the highest signal and then 

Clusters passing filters are those one that remain after the calculation of pass filter.

On the pattern flow cell there is a possibility of having, in addition to having polyclonal cluster


Quality Scores: estimate of the probabliity of error in base calling
Quality model:



Q30: what fraction of the reads should be better than Q30 (1 in 1000 error or 99.9% accuracy) 



Percent aligned and error rate
Spiking PhiX
% Aligned is the percent of clusters in which the first 25 cycles align to the PhiX reference genome
Error rate is the rate of mis-matches between sequencing data and PhiX reference genome

For low complexity libraries, spiking PhiX is recommended so that there is mixed material 

So lower the complexity, higher the spike-in of the PhiX

## Downstream Analysis Options

BaseSpace Sequence Hub
Local Run Manager

Have a reference guide for any instrument that you use handy. It can change quite frequently. Miseq: once every few moths, NovaSeq: quicker



# NovaSeq 


Data output: 65-3000Gb

There are four flow cells available.

SP: 0.4Tb
S1: 0.5Tb
S2: 1.25Tb
S4: 3Tb

Keep the used S4 flow cells handy. They can help with the wash

When you are transitioning to NovaSeq or a new platform what kind of determination would you make 
*Sequence Coverage Calculator*: to help not sequence any more than you need to and what kit to use

### Two workflows: 
Standard: Run one library pool across the 
XP: Run separate library in each lane

## Kit components
Cluster Cartridge
Library Tube
ExAmp Reagents
SBS Cartridge
Flow Cell
SP Manifold
Buffer Cartridge

### XP Components
Dock , Lane Kit

## 

Denature and Neutralize Library
Pooled input library 1-3nM
Final concentration of 250pM on S4 Flow Cell

