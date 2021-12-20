

## Detecting patterns in raster plots

In generic linear non linear lnl models, the output is assumed to be poisson As such a simple decoding strategy is to asscume it is to b inferned foran tuning curves (Jayazeri) or simply by a simple regression (Berens) This latter model aissunes a Bernouilt model for the generation of spites such that the decoding amounts to a single logistic regression.


### Paper by [@Grossberger2018]

* Temporally ordered multi-neuron patterns likely encode information in the brain. We introduce an unsupervised method, SPOTDisClust (Spike Pattern Optimal Transport Dissimilarity Clustering), for their detection from high-dimensional neural ensembles. SPOTDisClust measures similarity between two ensemble spike patterns by determining the minimum transport cost of transforming their corresponding normalized cross-correlation matrices into each other (SPOTDis).
* Detecting these temporal patterns represents a major methodological challenge.
* Many approaches to this problem are supervised, that is, they take patterns occurring concurrently with a known event, such as the delivery of a stimulus for sensory neurons or the traversal of a running track for hippocampal place fields, as a “template” and then search for repetitions of the same template in spiking activity :
 * Nadasdy Z, Hirase H, Czurko A, Csicsvari J, Buzsaki G. Replay and time compression of recurring spike sequences in the hippocampus. J Neurosci. 1999;19(21):9497–507. pmid:10531452
 * Lee AK, Wilson MA. A combinatorial method for analyzing sequential firing patterns involving an arbitrary number of neurons based on relative time order. J Neurophysiol. 2004;92(4):2555–73. pmid:15212425
 * Davidson TJ, Kloosterman F, Wilson MA. Hippocampal replay of extended experience. Neuron. 2009;63(4):497–507. pmid:19709631
* only one spike per neuron: fig 1A = "For each pattern and each neuron, a random position was chosen for the activation pulse."
 * t-SNE projection with HDBSCAN labels shows that our clustering method can retrieve all patterns from the data.
* data available @ https://doi.org/10.1371/journal.pcbi.1006283.s013


![Fig 1 of @Grossberger2018: "Simulated example illustrating the steps in SPOTDisClust. A) Structure of five “ground-truth” patterns (...). For each pattern and each neuron, a random position was chosen for the activation pulse. B) Neuronal output is generated according to an inhomogeneous Poisson process, with rates dictated by the patterns in (A)."](https://storage.googleapis.com/plos-corpus-prod/10.1371/journal.pcbi.1006283/2/pcbi.1006283.g001.PNG_L?X-Goog-Algorithm=GOOG4-RSA-SHA256&X-Goog-Credential=wombat-sa%40plos-prod.iam.gserviceaccount.com%2F20211206%2Fauto%2Fstorage%2Fgoog4_request&X-Goog-Date=20211206T141911Z&X-Goog-Expires=86400&X-Goog-SignedHeaders=host&X-Goog-Signature=e02aea1035ceeae4a9f78125ae56023b4175eff75b2b5ccf17df20242d3507c0ae38a4532e0d7f846545d70a69b8a9a4c7d04389aa190f71c71cdaaebe2790b4520135b30e5cfbce58cd00a1730e4c2347b01e81fbdf2ff1374cea9498c740df44087a56e7d143301656f1016432ea9cbf69b94dda26976f5db0597e10e215e340f5a59ca5fe4a33f45c8aae73b326206c97cb7a46cce97cfa0700555baa4b3925497c8a168454a49808c175015385277ea8edb794b7d7ac921c0833c27681ae9fc8301ed5e29da386fa0fc572ee490db1f5d93a938508fdcd20438c9d2bec19e64ef525471e41bbf7a1e14145f2ca8d71e02eb6c17ea681360628d563f7eee7){#fig:G2018-1 width="7in"}

### Russo et al 2017 [@Russo2017]

* "Here we present such a unifying methodological and conceptual framework which detects assembly structure at many different time scales, levels of precision, and with arbitrary internal organization. " by @Russo2017
* sliding window as in [@Grün2002] ("Numerous other statistical procedures for detecting assemblies or sequential patterns have been proposed previously") - extended to multiple lags [@Torre2016]
* based on a "non-stationarity-corrected parametric test statistic for assessing the independence of pairs" and "an agglomerative, heuristic clustering algorithm for fusing significant pairs into higher-order assemblies"

### Rastermap

* https://www.janelia.org/lab/stringer-lab
* described in [@Pachitariu2018]
* [rastermap](https://github.com/MouseLand/rastermap)
 * deconvolution strategy
 * based on a linear model

#### Stringer et al 2019, Nature [@Stringer2019nature]

* "A neuronal population encodes information most efficiently when its stimulus responses are high-dimensional and uncorrelated, and most robustly when they are lower-dimensional and correlated. Here we analysed the dimensionality of the encoding of natural images by large populations of neurons in the visual cortex of awake mice. "
* Data availability: All of the processed deconvolved calcium traces are available on [figshare](https://figshare.com/articles/Recordings_of_ten_thousand_neurons_in_visual_cortex_in_response_to_2_800_natural_images/6845348), together with the image stimuli.
* Code availability: The code is available on [GitHub](https://github.com/MouseLand/stringer-pachitariu-et-al-2018b).

#### Stringer et al 2019, Science [@Stringer2019science]

* Stringer et al. analyzed spontaneous neuronal firing, finding that neurons in the primary visual cortex encoded both visual information and motor activity related to facial movements. The variability of neuronal responses to visual stimuli in the primary visual area is mainly related to arousal and reflects the encoding of latent behavioral states.

* see also the work showing that you can encode very precise orientation information by using many neurons: [@Stringer2021]

#### Paper by [@Moser2014]

On Stability of Distance Measures for Event Sequences Induced by Level-Crossing Sampling