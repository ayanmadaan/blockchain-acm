# blockchain-acm

Structure of a block:

    1. Data
    2. Prev hash (64 digit hexadecimal number)
    3. Own hash
    4. Nonce (32 bit number)
    5. Timestamp

_**SHA-256**_  is used: think of this as a maths function f(x)=y, where y can be calculated if x is given, but not vice versa.

        Eg. If we aere asked to compute result of 2+3, we can do that =5, but if we are asked to produce the input for which our answer is 5, we can not do that cause they are so many cases.

A hash has 64 characters, 1 char = 4 bits, therefore size of a hash is 256 bits. And its a hexadecimal number.


Characteristics of a blockchain:

    1. An appropriate hash algo.
    2. P2P Network
    3. Consensus protocol


Now some applications are:

    1. Crypto Mining
    2. Mobile voting
    3. Immutable ledger
#




 ##  How Crypto mining works?

    1. Now the basic thing about a blockchain is that blocks are connected by a hasing algorithm.
    2. There's a particular target miners gotta keep in mind in order to mine a coin.
    3. In layman terms, one needs to score below the target to mine the block.
    4. We are presented with a 64 characters target with osme leading zeroes, and we keep changing our nonce an dwhen we get a hash below the target, voyla!


## Consensus Protocol

    1. Let's say there is a group of 4 friends and they're playing badminton.
    2. Me being the selfish being that I am, lie about the score to my friends in order that I am ahead.
    3. Now this could work if my friends are dumb, but I don't have dumb friends.
    4. So they ask each other what's the score and they reach to a consensus that I lied and then torture me good.
    5. That is consensus protocol and it works (personal experience).

## Proof of work

    I'm gonna keep this short, all of this I just explained above, combine them.

## Nonce Range

    1. Since nonce is a 32 bit number, it'll have 2^32 possibilities and one of them will be of our use.
    2. And hash is a 64 digit hexadecimal number, so its possibilities are 16^64.
    3. Following the rules of conditional probability, the probability we'll get both right is 10^-12.
    4. But that's not it, our block has one more part that we haven't talked about yet, TIMESTAMP.
    5. It changes every second and along with it, our hash also changes.
    6. F