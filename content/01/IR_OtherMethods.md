## Other Saturation-Recovery T<sub>1</sub> Mapping techniques

Several variations of the inversion recovery pulse sequence were developed to overcome challenges like those specified above. Amongst them, the Look-Locker technique {cite:p}`Look1970` stands out as one of the most widely used in practice. Instead of a single 90° acquisition per TR, a periodic train of small excitation pulses θ are applied after the inversion pulse, {θ<sub>180</sub> – 𝛕 – θ – 𝛕 – θ – ...}, where  𝛕 = TR/n and n is the number of sampling acquisitions. This pulse sequence samples the inversion time relaxation curve much more efficiently than conventional inversion recovery, but at a cost of lower SNR. However, because the magnetization state of each TI measurement depends on the previous series of θ excitation, it has higher sensitivity to B<sub>1</sub>-inhomogeneities and imperfect spoiling compared to inversion recovery {cite:p}`Gai2013,Stikov2015`. Nonetheless, Look-Locker is widely used for rapid T<sub>1</sub> mapping applications, and variants like MOLLI (Modified Look-Locker Inversion recovery) and ShMOLLI (Shortened MOLLI) are widely used for cardiac T<sub>1</sub> mapping {cite:p}`Messroghli2004,Piechnik2010`.

Another inversion recovery variant that’s worth mentioning is saturation recovery, in which the inversion pulse is replaced with a saturation pulse: {θ<sub>90</sub> – TI – θ<sub>90</sub>}. This technique was used to acquire the very first T<sub>1</sub> map {cite:p}`Pykett1978`. Unlike inversion recovery, this pulse sequence does not need a long TR to recover to its initial condition; every θ<sub>90</sub> pulse resets the longitudinal magnetization to the same initial state. However, to properly sample the recovery curve, TIs still need to reach the order of ~T<sub>1</sub>, the dynamic range of signal potential is cut in half ([0, M<sub>0</sub>]), and the short TIs (which have the fastest acquisition times) have the lowest SNRs.

```{admonition} References
:class: seealso

```{bibliography}
:filter: docname in docnames
```

```