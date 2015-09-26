searchers
=========

This crate provides various implementations of the `std::str::patter::Searcher` trait. It's general philosophy is:

 - the speed of `next_match()` is important, but the speed of `next()` and `next_reject()` are not.
 - preprocessing time is not important; searching speed is.
 - if some special case can be done faster, then we will provide an implementation for that special case.

