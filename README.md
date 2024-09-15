Implementation of various sorting algorithms in Rust

```rust
$ cargo r --release > values.dat
$ sed -i '' '1s/^/algorithms n comparisons\n/' values.dat
$ R
t <- read.table('values.dat', header=TRUE)
library(ggplot2)
ggplot(t, aes(n, time, colour = algorithm)) + geom_point() + geom_smooth()
```
