# a-hist
a wrong hist i met, wonder if its a bug of pytorch 

```python
>>> import torch
>>> hist = torch.load('hist.pth')
>>> hist.sum()
tensor(21956292.)
>>> sum(hist)
tensor(21956260.)
>>> sum(hist[2:]) + sum(hist[:2])
tensor(21956264.)
>>> hist[2:].sum() + hist[:2].sum()
tensor(21956296.)

```
why these value are not the same???
