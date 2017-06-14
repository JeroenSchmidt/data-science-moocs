[TOC]

# Converting

## Factor -> Numeric

[See link](https://stackoverflow.com/questions/3418128/how-to-convert-a-factor-to-an-integer-numeric-without-a-loss-of-information)

Using `as.Numeric` will convert the Factor keys. *Solution:*

```R
as.numeric(levels(f))[f]
```

OR

```
as.numeric(as.character(f))
```

where `f` is your dataset/dataframe$col