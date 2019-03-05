
## 5 mar (how to write a paper & reseach)

We might be able to create a [graphical abstract](https://www.elsevier.com/authors/journal-authors/graphical-abstract)


[How to read a paper](https://www.albany.edu/spatial/WebsiteFiles/ResearchAdvices/how-to-read-a-paper.pdf) might be useful.

#### [PDF](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/07/How-to-write-a-great-research-paper.pdf) about writing a paper (nice).

This pdf explains the way to write a paper, we can use these techniques.

- intro
 - list our contributions and the reasons our contributions are important
 - hook the reader with interesting content (anecdote?) 
- body
 - explain/prove the claims made in the introduction
 - evidence about those claims are: comparisons/theorem/case studies

**main takeaway**:

1. Don’t wait: write
2. Identify your key idea
3. Tell a story
4. Nail your contributions
5. Related work: later
6. Put your readers first (examples)
7. Listen to your readers


### Research.. 

didnt check this one yet: https://ieeexplore-ieee-org.tudelft.idm.oclc.org/stamp/stamp.jsp?tp=&arnumber=8634961  
source: scopus query: `( TITLE-ABS-KEY ( smart  AND contract ) )  AND  ( platforms ) ` 3rd res

also didnt check https://ieeexplore-ieee-org.tudelft.idm.oclc.org/stamp/stamp.jsp?tp=&arnumber=8394569  
source: ieeexplore query: [smart contract platforms](https://ieeexplore-ieee-org.tudelft.idm.oclc.org/search/searchresult.jsp?newsearch=true&queryText=smart%20contract%20platforms)


[Study on smart contract research.](https://www-sciencedirect-com.tudelft.idm.oclc.org/science/article/pii/S0736585318308013)
Seems very useful. found on Scopus, query: `( TITLE-ABS-KEY ( smart  AND contract ) )  AND  ( ( ( platforms ) )  AND  ( randomness ) )  AND  ( survey )`

https://ieeexplore-ieee-org.tudelft.idm.oclc.org/Xplore/home.jsp

## 3 mar (topic and smart contract env)

[Blockchains and Smart Contracts for the Internet of Things](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7467408)
Legal enforceability of smart contracts is limited. Work
is being done [84]) to make the technical rules of smart
contracts legally enforceable and binding to all parties. 


search: ("smart contract" "applications" "consensus" "transactions" "future") google scholar

[overview of smart contracts](http://ir.ia.ac.cn/bitstream/173211/21809/1/An%20overview%20of%20smart%20contract%20Architecture%2C%20applications%2C%20and%20future%20trends.pdf)

[overview of blockchain](file:///C:/Users/nickd/Downloads/5dd6abe30d6f850c05d1036a3a5791dad63357e4.pdf)

search ^ + "traditional"

[Understanding Modern Banking Ledgers through Blockchain
Technologies: Future of Transaction Processing and Smart
Contracts on the Internet of Money](https://arxiv.org/pdf/1511.05740.pdf)

[smart contract Triplicate](https://www.researchgate.net/profile/Peter_Eze7/publication/317349621_A_Triplicate_Smart_Contract_Model_using_Blockchain_Technology/links/5937782c4585158f6464595f/A-Triplicate-Smart-Contract-Model-using-Blockchain-Technology.pdf)

[lottery, cant read?](https://ieeexplore.ieee.org/abstract/document/8181505)


Research question directions:

smart contracts:

- future directions
- applications
- security
- scalability and limits
- incentives



## 1 mar (not much)

read [Blockchain challenges and opportunities: a survey](https://www.henrylab.net/pubs/ijwgs_blockchain_survey.pdf)



## 26/27 feb (smart contract platforms)

### Smart contract platforms

look into: bitshares, hyperledger

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
## 25/26 feb (initial research)

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
## 24 feb (initial research)


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
hash and a size..
