Photometric Transformation Equations for the Vera C. Rubin Observatory

Abstract

Astronomical survey systems are used around the world to collect data
from the surrounding cosmic neighborhood and beyond. Different optical
filters are used to collect different kinds of data, and each survey
system uses its own filters specified for its mission. The
transformation equations provided in this thesis help to begin
bridging the gaps between filter systems, allowing more data to be
used overall.

Authors

Meagan Porter (First Author)

Douglas Tucker (Corresponding Author)

J. Allyn Smith

Christina Adair

Jeff Carlin

Formatting Reference

The structure and formatting of this Technical Note follow the style
of the Dark Energy Survey Data Release 2 photometric transformation
relations, available at:
https://des.ncsa.illinois.edu/releases/dr2/dr2-docs/dr2-transformationsns

DES to LSST Synthetic

Representative stellar magnitudes were derived by integrating
spectrophotometric spectra from the Pickles Stellar Spectra Library
[Pickles:1998] with filter passband transmission curves for the DES
and LSST systems. These synthetic magnitudes were calculated using the
broad-band absolute magnitude definitions, as given by established
equations for flux integration across response function for each
filter.

The resulting synthetic data were then processed using a Python-based
fitting code to generate transformation equations between filter
systems. Due to the limited number of stars in the Pickles library
(approximately 100), the resulting plots are relatively sparse. These
are shown in Figures 1–4. However, the synthetic approach allows for a
consistent and controlled method for deriving magnitude
transformations across different survey filter sets, providing a
useful reference for photometric calibration and comparison.


g_{\rm LSST} = g_{\rm DES} + 0.016 (g - i)_{\rm DES} - 0.003(g - i)^2_{\rm DES} + 0.006 \quad \text{(RMS: 0.002 mag)}\\
r_{\rm LSST} = r_{\rm DES} + 0.185 (r - i)_{\rm DES} - 0.015(r - i)^2_{\rm DES} + 0.010 \quad \text{(RMS: 0.008 mag)}\\
i_{\rm LSST} = i_{\rm DES} + 0.150 (r - i)_{\rm DES} - 0.003(r - i)^2_{\rm DES} - 0.009 \quad \text{(RMS: 0.005 mag)}\\
z_{\rm LSST} = z_{\rm DES} + 0.270 (i - z)_{\rm DES} + 0.036(i - z)^2_{\rm DES} - 0.003 \quad \text{(RMS: 0.010 mag)}


The DES to LSST transformation equations apply to stars with
magnitudes that are roughly within the range (-0.8 < g-i < 2.6) for
(g)-band, (-0.4 < r-i < 1.2) for (r) and (i)-band, and (-0.3 < i-z <
0.6) for (z)-band. These were computed using approximately 420 stars
spread across 10 nights during three observing runs in 2024. Due to
the relatively few stellar observations in this data set, the plots
appear to be sparse, and the total span of the color range is small
compared to the plots in the other sections. However, the fits are
robust considering the amount of data, and the RMS of the residuals is
well within the anticipated range.









