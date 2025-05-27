# Fermi-LAT 12-years all-sky gamma-ray maps 

This repository contain the Fermi-LAT all-sky Gamma-Ray maps used in the cross-correlation analysis performed by [Thakore et. al. (2025)](https://arxiv.org/pdf/2501.10506) between the tangential shear obtained from the DES Y3 survey (data available from [DES Data Management](https://des.ncsa.illinois.edu)) and 12-year gamma-ray data from the [Fermi Large Area Telescope (LAT)](https://fermi.gsfc.nasa.gov). We refer to the aforementioned paper for the details regarding the generation of the gamma-ray maps, as well as to [Ackermann et al. 2019](https://arxiv.org/abs/1812.02079) for additional tests. The main characterisitcs of these maps are listed below.

## The Maps 

Each .zip file contains a (NSIDE=1024) map in one of the nine energy bins detailed in the paper (and generated from 100 micro, logarithmically spaced bins between 100 MeV and 1 TeV), with the gamma-ray energy range split between 631 MeV to 1 TeV. The indices in the  filenames range from 0 to 8 and correlate to each energy bin as follows:
  - Index 0 : 631 MeV to 1.202 GeV
  - Index 1 : 1.202 GeV to 2.290 GeV
  - Index 2 : 2.290 GeV to 4.786 GeV
  - Index 3 : 4.786 GeV to 9.12 GeV
  - Index 4 : 9.12 GeV to 17.38 GeV
  - Index 5 : 17.38 GeV to 36.31 GeV
  - Index 6 : 36.31 GeV to 69.18 GeV
  - Index 7 : 69.18 GeV to 131.8 Gev
  - Index 8 : 131.8 GeV to 1.00 TeV

>[!Note]
> - The maps are masked, with a energy-dependent mask (as detailed in [Thakore et. al. (2025)](https://arxiv.org/pdf/2501.10506) and [Ackermann et al. 2019](https://arxiv.org/abs/1812.02079)). The masked puxels are rendered with a pixel is set to the healpy UNSEEN value.
> - The maps are integrated flux maps in the different enerrgy bins, in units of $cm^{-2} s^{-1} sr^{-1}$, foreground subtracted (see details in [Ackermann et al. 2019](https://arxiv.org/abs/1812.02079)).

>[!Caution]
>It is not advised to use these maps to different types of analyses different from auto/cross-correlations like [Ammazzalorso et al 2018](https://arxiv.org/abs/1808.09225), [Ackermann et al. 2019](https://arxiv.org/abs/1812.02079), [Ammazzalorso et al 2020](https://arxiv.org/abs/1907.13484), [Thakore et. al. (2025)](https://arxiv.org/pdf/2501.10506), [Negro et al 2022](https://arxiv.org/abs/2304.10934)

