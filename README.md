Implementation of various sorting algorithms in Rust

```rust
$ cargo r --release > values.dat
$ sed -i '' '1s/^/algorithm n comparisons\n/' values.dat
$ R
t <- read.table('values.dat', header=TRUE)
library(ggplot2)

# to plot # comparisons
ggplot(t, aes(n, comparisons, colour = algorithm)) + geom_point() + geom_smooth()
```
