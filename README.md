# Grids

A mixin to help create Gridset style grids.

## Warning

Depending on how many grids you have, these can take a while to compile with Sass (10-15 seconds).

## Helper functions

To help store your grid dimensions, it is suggested what you make use of the following functions:

``` sass
// grid dimensions
@function grid-cols($prefix){
  @if $prefix == s  { @return (11.212121212121213,32.7878787878788,32.7878787878788,11.212121212121213); }
  @if $prefix == m  { @return (11.212121212121213,16.2689393939394,16.2689393939394,16.2689393939394,16.2689393939394,11.212121212121213); }
  @if $prefix == mb { @return (11.212121212121213,22.5252525252525,22.5252525252525,22.5252525252525,11.212121212121213); }
  @if $prefix == l  { @return (11.212121212121213,16.8939393939394,16.8939393939394,16.893939393939394,16.8939393939394,11.212121212121213); }
  @if $prefix == lb { @return (11.212121212121213,23.1919191919192,23.1919191919192,23.1919191919192,11.212121212121213); }
  @if $prefix == lc { @return (11.212121212121213,11.212121212121213,22.5505000407102,22.5505000407102,11.212121212121213,11.212121212121213); }
}

@function grid-gutter($prefix){
  @if $prefix == s  { @return 4; }
  @if $prefix == m  { @return 2.5; }
  @if $prefix == mb { @return 2.5; }
  @if $prefix == l  { @return 2; }
  @if $prefix == lb { @return 2; }
  @if $prefix == lc { @return 2; }
}
```