# Public data products

### Paper: The atomic gas sequence and mass-metallicity relation from dwarfs to massive galaxies
**Link: [Scholte et al. (2024)](https://ui.adsabs.harvard.edu/abs/2024arXiv240803996S/abstract)**

#### Atomic gas sequence
Measurements of the atomic gas sequence for a mass complete sample of galaxies: [Download here](https://github.com/dirkscholte/dirkscholte.github.io/blob/main/BPT_diagrams.png "download").

You can use the function below to plot the function we fitted to the data:
```python
def logfhi(logM, gamma0=-0.391854, gamma1= -0.75324106, beta=1.46898262, M0=9.29457064,logfhi7=1.02060954):
    '''The atomic gas sequence of a mass complete sample of galaxies.'''
    return logfhi7 + gamma0*np.log10((10**logM)/(10**7)) + (gamma1-gamma0)/beta * np.log10(1+((10**logM)/(10**M0))**beta)
```
#### Mass-metallicity relation
Measurements of the mass-metallicity relation for an emission line flux limited sample of galaxies: [Download here]().

You can use the function below to plot the function we fitted to the data:
```python
def mzr(mstar, Z0=8.854, M0=10.49, gamma1=0.2439, beta0=1.21):
    '''The mass-metallicity relation for an emission line flux limited sample'''
    return Z0 - gamma1/beta0 * np.log10(1+(10**mstar/(10**M0))**-beta0)

```

Measurements of the mass-metallicity relation for a mass complete sample: [Download here]().

### Paper: Cold gas mass measurements for the era of large optical spectroscopic surveys
**Link: [Scholte & Saintonge (2023)](https://ui.adsabs.harvard.edu/abs/2023MNRAS.518..353S/abstract)**

Grids of photoionization models: [Download here](https://oup.silverchair-cdn.com/oup/backfile/Content_public/Journal/mnras/518/1/10.1093_mnras_stac3134/1/stac3134_supplemental_files.zip?Expires=1727870456&Signature=gUryeNQY-g~tLWWSn8b2TV4~Nm3cNZs5zdvLxdrK~5u18smqV~JAX2VxRICqrY2FTCGlg5oTmpDncURx0hToq7BKqsFbe6XXtE0SQMNT6jUF-tVEP4lrPyOae8h1s0coZOF65SZZwFoEKwbH~loF-aav4~GeUz7gQwE3UXBOM0O3yaPu6XAZfz71asY1KDuDzOXyfzgK8P4EMBebb2bE7ngNfWyc7yBw2Lj33dni43H0NLNCSkZuR~PSQeSWZhYBl4fXmJ7EiUqkm3mon7JxRjsijNGct6bR29-PsDjs0vBuytTv8C-ScoJDbz-vEeho5MsrCbU47TAtta8jVdl1dw__&Key-Pair-Id=APKAIE5G5CRDK6RD3PGA).
