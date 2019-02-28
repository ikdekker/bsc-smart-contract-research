
## 26/27 feb

### Smart contract platforms

#### Ethereum..

#### [EOS](https://blockgeeks.com/guides/eos-blockchain/) [paper](https://github.com/EOSIO/Documentation/blob/master/TechnicalWhitePaper.md)

**About**

The EOS blockchain claims to be capable of millions of transactions per second.
Block production is done by picking 21 producers every 0.5 seconds. 21 unique
producers will be picked 6 times per round. So a consensus is arrived at every 3
seconds. Token holders cast their vote on which candidates in the network they
trust as a producer.

**Features**

* no transaction fees
* decentralized OS for Dapps
* voting on other nodes (Delegated PoS)
* incentiviced to stay in the voting process
* inflation rate to reward the workers
* C/C++ for smart contracts ([fun tutorial](https://battles.eos.io/tutorial/lesson1/), which i don't want to invest time in atm)



#### [Codius](https://github.com/codius/codius-wiki/wiki/White-Paper)

*About*

* Smart Oracle
* 



#### [Stellar (Ripple Fork)](https://www.stellar.org/how-it-works/stellar-basics/) ([paper](https://www.stellar.org/papers/stellar-consensus-protocol.pdf))

**About**

Stellar consensus protocol(SCP) gives each node freedom to choose other nodes
which it trusts.

**Features**

* uses anchors to remove trust
* SCP (supposed to be safe, decentralized, low-latency & trustworthy)


**conclusion**

I believe both EOS and Stellar are capable of multi-currency transactions. Where
two people can trade different currencies seamlessly.

-----
## 25/26 feb

### <a id='eoe'>Evolution of Ethereum</a>
#### related [devcon talk](https://www.youtube.com/watch?v=Yo9o5nDTAAQ&feature=youtu.be&t=7h55m40s)

Ethereum has four main stages planned. Three of which have already been
(partially) implemented. Each hard stage is released with a hard fork, changing
the functionality of contracts. These changes are not backward compatable. The
four stages are codenamed Frontier, Homestead, Metropolis, and Serenity. Some of
these stages contain subreleases, like with Metropolis. Byzantium, which has
already been released in 2017 and Constantinople, due to be released this week,
28 feb. It has been postponed before for security reasons. 

#### Ethereum challenges for Constantinople & further

Major challenges in Ethereum are: privacy (decentralization), security and
scalability. Two of these are "easily" solvable, but it is harder to solve all
three. The biggest flaw of most blockchains is that they are as fast as their
individual nodes. This causes a huge bottleneck when a blockchain grows large.
To solve the trilemma, Ethereum can sharded into multiple systems of nodes. The
approach they want to take is called quadratic sharding. Each node works on the
shard-network it is interested in, and the combination of all shard-networks.
Therefore, it takes quadratic time to add a block. This sharded Ethereum would
allow for many more transactions per second, allowing a more wide-spread
adoption.

Also good to know about: [Ethereum Casper](https://blockgeeks.com/guides/ethereum-casper/)
..expand on casper..

casper ffg https://arxiv.org/pdf/1710.09437.pdf

#### About sharding [(Ethereum wiki on sharding)](https://github.com/ethereum/wiki/wiki/Sharding-FAQs)

Sharding is the act of splitting up a resource to increase its speed. For
instance, a large database can be split into multiple databases and scaled
across multiple servers. The same principle can be used with Ethereum. See
[Evolution of Ethereum](#eoe).

----
## 24 feb


### Proof of Stake

A security deposit is made by all validators -> if you submit an invalid block,
your deposit will be taken. Earlier versions of PoS only required people to own
the currency. This ownership was taken as the "stake". However, using this
method, attackers could submit false blocks without risking anything. The idea
was that when someone had an investment in a currency, their own wealth would be
compromised. Since you have more at stake when you have more wealth, this is
considered proof of stake.

When paying (yourself) as result of a stake, the coin age is consumed. This is
desired, since it stops PoS from favouring people with a high coin age to win
consecutively and therefore, decentralizing the network.

Proof of Stake still requires the Proof of Work mechanism, to allow coins to
enter the circulation. Since there are not enough coins owned by various in the
early stages of a coin, the coins need to be minted(and transactions verified)
in an alternative fashion. After a good distribution has been achieved, the 
proof-of-work can be replaced by the stake.


### IPFS - [InterPlanetary FileSystem](file:///D:/Downloads/ipfs-p2p-file-system.pdf)

IPFS allows for sharing files on a global scale without a centralized server.
Files are mostly not stored as a whole, but are distributed. A file, larger than
the maximum chunk size, will be split up in several pieces. The pieces have a name,
hash and a size