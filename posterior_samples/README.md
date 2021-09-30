# Posterior samples

This directory contains the event posterior samples
* posteriors_1.pkl, posteriors_2.pkl (spinning)
* posteriors_zero_1.pkl, posteriors_zero_2.pkl (non-spinning) 


To read in the posterior files use the following:

```bash
import pandas as pd

posts = pd.read_pickle("posteriors_1.pkl") + pd.read_pickle("posteriors_2.pkl")
posts_zero = pd.read_pickle("posteriors_zero_1.pkl") + pd.read_pickle("posteriors_zero_2.pkl")

event_ids = []
ff = open("event_list.txt","r")
for line in ff.read().splitlines():
    event_ids.append(line)
```

where the corresponding	event name can be found	under the same index of the `event_ids` list.
