### QuickCheck

As part of that I also learned how to use newtypes to wrap existing types to
define monoid instances for the newtypes b/c the types they wrap could have multiple
valid Monoid instance.

## Topics of Interest
The Haskell topics I 
am most interested in are parser combinators (a purely functional way to build
parsers, which are used by libraries like [parsec](https://wiki.haskell.org/Parsec) 
& [attoparsec](https://hackage.haskell.org/package/attoparsec), and [monad
transformers](https://hackage.haskell.org/package/mtl) which, seem to be required
knowledge to be able to use the parser libraries, the stream processing library 
[pipes](https://github.com/Gabriel439/Haskell-Pipes-Library/blob/master/benchmarks/LiftBench.hs), and the web framework [scotty](https://github.com/scotty-web/scotty/blob/master/examples/reader.hs.).

I am also very interested in [Servant](https://haskell-servant.github.io/) 
(a web framework which has a type level DSL for client & documentation 
generation) and [Haxl](https://hackage.haskell.org/package/haxL), a concurrent 
programming library.


I have broken ground on my bittorrent client, got a bencode decoder working and
tested last week. This week I plan on finishing the encoder portion (using
vanilla haskell i.e. no parser combinators) so I can get started on the networking
portion of the bittorrent client.  Once I learn parser combinators I will refactor
the parser to use then.

I am very interested in distributed hash table protocols and how they work.
Last week I read the [chord paper](https://pdos.csail.mit.edu/papers/chord:sigcomm01/chord_sigcomm.pdf)
on Brian Mitchell's suggestion and it was a great introduction to the topic.  It
describes the Chord DHT protocol used in casandra. I found that the bittorrent
magnet links use the Kademlia protocol, which I read about last week as well
https://pdos.csail.mit.edu/~petar/papers/maymounkov-kademlia-lncs.pdf.

I ended learning a ton from that paper including the concept of a metric (in
group theory) and how XOR on binary string is sufficient to construct a metric
which can be used to drive  concensus in the network rearding where to find
key / value pairs.  I gave a talk on it this monday, the slides for which can
be found [here](https://docs.google.com/presentation/d/1yZZOjIm0isexTe2bkEFh7_22w5Z_dTiRd_sU9q4yGCs/edit?usp=sharing). I have been trying to push my comfort level 


