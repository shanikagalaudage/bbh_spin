# Hyper-posterior samples

This directory contains the hyper-posterior samples for the _Extended_ model analysis.
For results for the _Default_ spin model results as in [LVC GWTC-2 population analysis](https://arxiv.org/abs/2010.14533), see the official data release from LIGO/Virgo [here](https://dcc.ligo.org/LIGO-P2000434/public) in `Population_Samples.tar.gz`

## Reading samples

You can read in the samples using either of the following methods:

If you have [`bilby`](https://git.ligo.org/lscsoft/bilby/-/tree/master/bilby) installed,

```bash
>>> from bilby.core.result import read_in_result

>>> result = read_in_result("mass-powerlawpeak_spin-extended.json")
>>> posterior = result.posterior
>>> posterior.keys()
Index(['alpha', 'beta', 'mmax', 'mmin', 'lam', 'mpp', 'sigpp', 'delta_m',
       'mu_chi', 'sigma_chi', 'lambda_chi_peak', 'xi_spin', 'sigma_spin',
       'zmin', 'lamb', 'amax', 'log_likelihood', 'log_prior'],
      dtype='object')
```

if you don't have `bilby` you can access the samples as follows,

``` bash
>>> import json

>>> fobject = open("mass-powerlawpeak_spin-extended.json","r")
>>> data = json.load(fobject)
>>> posterior = data['posterior']['content']
>>> posterior.keys()
dict_keys(['alpha', 'beta', 'mmax', 'mmin', 'lam', 'mpp', 'sigpp', 'delta_m', 
           'mu_chi', 'sigma_chi', 'lambda_chi_peak', 'xi_spin', 'sigma_spin',
           'zmin', 'lamb', 'amax', 'log_likelihood', 'log_prior'])
```
