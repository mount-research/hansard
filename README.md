
Hansard
========

[![crates.io version](https://img.shields.io/crates/v/hansard.svg)](https://crates.io/crates/hansard)

At the moment just grabs the last 20 [Hansard Bound Volumes](http://api.data.parliament.uk/resources/files/feed?dataset=14) zipfiles.

Usage:

`hansard all` Gets the last 20 bound volumes and saves to ./data/ directory

`hansard xml` Prints the xml from the last 20 bound volumes e.g `hansard xml | grep election`

Usage as library:
```rust
    extern crate hansard;

    use hansard::retrieve;

    fn main(){
        // call retrieve to start the download of the bound volumes
        retrieve::retrieve();
    }
```

[License](https://github.com/mount-research/hansard/blob/master/LICENSE.md)
