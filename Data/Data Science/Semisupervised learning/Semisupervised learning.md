---
tags:
  - machine-learning
  - semisupervised-learning
---

Algorithms that can deal with data that are partially [[Training set#Label|labelled]].

most semisupervisied learning algorithms are combinations of [[Unsupervised learning]] and [[Supervised learning]] algorithms. 

## Examples
- [Deep belief networks](https://en.wikipedia.org/wiki/Deep_belief_network)
	- Based on [[Unsupervised learning]] components called [restricted Boltzmann machines](https://en.wikipedia.org/wiki/Restricted_Boltzmann_machine) stacked on top of one another. 
	- [RBM](https://en.wikipedia.org/wiki/Restricted_Boltzmann_machine) are trained sequentially in an [[Unsupervised learning|unsupervised]] manner, and then the whole system is fine-tuned using [[Supervised learning|supervised learning]] techniques.
## Services examples that uses supervised learning
- [Google Photos](https://photos.google.com/?pli=1)
	- Once you upload your family photos to the service, it automatically recognizes that the same person A shows up in some photos, while another person B shows up in some other photos. This is the [[Unsupervised learning]] part of the algorithms ([[Clustering]]). Now you would need to tell the system who some of these people are ([[Training set#Label|Labelling]])

