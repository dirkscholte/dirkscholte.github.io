# Public data products

### Paper: The atomic gas sequence and mass-metallicity relation from dwarfs to massive galaxies
**Link: [Scholte et al. (2024)](https://ui.adsabs.harvard.edu/abs/2024arXiv240803996S/abstract)**

#### Atomic gas sequence
Measurements of the atomic gas sequence for a mass complete sample of galaxies: 
<a href="https://github.com/dirkscholte/dirkscholte.github.io/raw/main/data/scholte24_mass_complete_fhi_sequence.fits" download="true" data-testid="raw-button" data-loading="false" data-no-visuals="true" data-size="small" aria-describedby=":R5csptal9lab:-loading-announcement" class="types__StyledButton-sc-ws60qy-0 jUNlHb" data-hotkey="Meta+/ Meta+r"><span data-component="buttonContent" class="Box-sc-g0xbh4-0 kkrdEu"><span data-component="text">Download here</span></span></a>.

You can use the function below to plot the function we fitted to the data:
```python
def logfhi(logmstar, gamma0=-0.14, gamma1= -0.854, beta=1.2, M0=8.98,logfhi7=0.45):
    '''The atomic gas sequence of a mass complete sample of galaxies.'''
    return logfhi7 + gamma0*np.log10((10**logmstar)/(10**7)) + (gamma1-gamma0)/beta * np.log10(1+((10**logmstar)/(10**M0))**beta)
```
#### Mass-metallicity relation
Measurements of the mass-metallicity relation for an emission line flux limited sample of galaxies:
<a href="https://github.com/dirkscholte/dirkscholte.github.io/raw/main/data/scholte24_line_flux_limited_mzr.fits" download="true" data-testid="raw-button" data-loading="false" data-no-visuals="true" data-size="small" aria-describedby=":R5csptal9lab:-loading-announcement" class="types__StyledButton-sc-ws60qy-0 jUNlHb" data-hotkey="Meta+/ Meta+r"><span data-component="buttonContent" class="Box-sc-g0xbh4-0 kkrdEu"><span data-component="text">Download here</span></span></a>.


You can use the function below to plot the function we fitted to the data:
```python
def mzr(logmstar, Z0=8.854, M0=10.49, gamma1=0.2439, beta0=1.20):
    '''The mass-metallicity relation for an emission line flux limited sample'''
    return Z0 - gamma1/beta0 * np.log10(1+(10**logmstar/(10**M0))**-beta0)
```

Measurements of the mass-metallicity relation for a representative sample of star-forming galaxies:
<a href="https://github.com/dirkscholte/dirkscholte.github.io/raw/main/data/scholte24_representative_mzr.fits" download="true" data-testid="raw-button" data-loading="false" data-no-visuals="true" data-size="small" aria-describedby=":R5csptal9lab:-loading-announcement" class="types__StyledButton-sc-ws60qy-0 jUNlHb" data-hotkey="Meta+/ Meta+r"><span data-component="buttonContent" class="Box-sc-g0xbh4-0 kkrdEu"><span data-component="text">Download here</span></span></a>.

### Paper: Cold gas mass measurements for the era of large optical spectroscopic surveys
**Link: [Scholte & Saintonge (2023)](https://ui.adsabs.harvard.edu/abs/2023MNRAS.518..353S/abstract)**

Grids of photoionization models: [Download here](https://oup.silverchair-cdn.com/oup/backfile/Content_public/Journal/mnras/518/1/10.1093_mnras_stac3134/1/stac3134_supplemental_files.zip?Expires=1727870456&Signature=gUryeNQY-g~tLWWSn8b2TV4~Nm3cNZs5zdvLxdrK~5u18smqV~JAX2VxRICqrY2FTCGlg5oTmpDncURx0hToq7BKqsFbe6XXtE0SQMNT6jUF-tVEP4lrPyOae8h1s0coZOF65SZZwFoEKwbH~loF-aav4~GeUz7gQwE3UXBOM0O3yaPu6XAZfz71asY1KDuDzOXyfzgK8P4EMBebb2bE7ngNfWyc7yBw2Lj33dni43H0NLNCSkZuR~PSQeSWZhYBl4fXmJ7EiUqkm3mon7JxRjsijNGct6bR29-PsDjs0vBuytTv8C-ScoJDbz-vEeho5MsrCbU47TAtta8jVdl1dw__&Key-Pair-Id=APKAIE5G5CRDK6RD3PGA).
