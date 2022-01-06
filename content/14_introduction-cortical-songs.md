

### precise temporal patterns TODO read [@Luczak2015]

[@Luczak2015] Luczak A, McNaughton BL, Harris KD. Packet-based communication in the cortex. Nat Rev Neurosci. 2015;16(12):745–55.


### cortical songs [@Ikegaya2004]

* Ikegaya and colleagues worked on spontaneous activity in vitro and in vivo. They demonstated that in cortical activity, we can find a repetition of several motifs. In PSCs, but also in spike activity. These sequences repeat after minutes and have a precise spatio temporal structure with a ms precision. They can be specific of a particular layer or colomn, are synchronized with network activity oscillation and can involve several cells. They also demonstated that these sequences can form supersequences : the cortical songs. It consist of the assembly of several sequences which repeat in a specific order with a compressed timing.


* "We find precise repetitions of spontaneous patterns of synaptic inputs in neocortical neurons in vivo and in vitro. These patterns repeat after minutes, maintaining millisecond accuracy."
* Precisely repeating motifs of spontaneous synaptic activity in slices: duration around 1s +/- .5 s. Some events in motifs are of similar size but sometimes absent - better described by Bernouilli than SE (and covariance)
* *in vivo*  spontaneous activity also reveals repeating sequences. About 3000 sequences, each involving 3-10 cells out of about 900, and last up to 3 seconds
* topography: "Sequences had specific topographic structures, in some cases involving only a particular layer or a vertical column of cells or cells located in a cluster (Fig. 4, A and B, and fig. S3B). (...) Therefore, repeating temporal patterns of activation (...) were associated with a structured spatial organization of the neurons that formed them."
* "Cortical songs: modular assemblies of repeated sequences": hierarchical detection.
* in cotical songs, there is a "compressing timing" which may be taken into account by a similar mechanism as maxpooling in CNNs for space, but in time. Or there may be a mechanism for controlling the replay speed (pulvinar, ... ,  ?)

![Fig. 1. from  [@Ikegaya2004] Repeated motifs of spontaneous synaptic activity in vitro and in vivo. (A) Repeated motifs of intracellular activity from layer 5 pyramidal neurons in slices. Panels show segments (red) of the same voltage-clamp recording from the same cell repeating seconds or minutes after the initial occurrence (blue). Arrows indicate timings of repeated PSCs. (i) Upper trace: low–temporal resolution display of spontaneous activity of a neuron. Lower traces: higher resolution display of the repeated motif at indicated regions of the trace (a to c). (ii) Example of a longer motif. (B) Three repetitions of a motif. The top traces show the motifs superimposed on each other (blue, green, and red), the middle traces show these same traces individually, and the bottom traces show temporally magnified regions of the motifs (a to c). (C) Repeated sequences of intracellular current-clamp recordings in vivo. Two (i) and three (ii) repetitions of motifs are shown. Shuffle tests were performed on traces (i), a to c, yielding significantly fewer repeats (fig. S2, P < 0.02). In (i), the blue trace is shifted –2.75 mV; in (ii), the blue trace is shifted –1.58 mV, and the green +0.79 mV.](images/Ikegaya2004zse0150424620001.jpeg)


It is interesting to make a parallel with the "Rapid Formation of Robust Auditory Memories" reported in [@Agus2010] which uses noise patterns. They " used random waveforms to probe the formation of new memories for arbitrary complex sounds. A behavioral measure was designed, based on the detection of repetitions embedded in noises up to 4 s long." The  task is to detect the repetition of the same (frozen) noise within a trial. " Unbeknownst to listeners, some noise samples reoccurred randomly throughout an experimental block." they showed that the "repeated exposure induced learning for otherwise totally unpredictable and meaningless sounds" by showing that the sensitivity increases in that case. Note that "acoustical analyses failed to reveal any obvious differences between good and bad noises" and that "Time reversal had no significant effect on the RefRN advantage" (quite surprising). The Learning is unsupervised (statistical, automatic), fast-acting (phase transition, "insight"), and long-lasting (memorization).

### polychronization