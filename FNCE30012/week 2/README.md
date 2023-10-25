# Regulated Payment Systems
1. <details>
   <summary>What is the primary function of Swift in the regulated payment systems?</summary>
   A messaging platform that links more than 11,000 financial institutions globally, providing a secure, reliable, and trusted communication channel.
   </details>

2. <details>
   <summary>Does Swift hold funds, manage accounts, or transfer money directly?</summary>
   No, Swift does not hold funds, manage accounts, or transfer money directly.
   </details>

3. <details>
   <summary>How does Swift generate revenue, and what was its revenue in 2022?</summary>
   Swift generates revenue through its services, and its revenue was 947 million EUR in 2022.
   </details>

4. <details>
   <summary>How are financial institutions identified within the Swift network?</summary>
   Each financial institution is identified by a code structured as <bank-id><country><branch>. For example, a CBA branch may have the code CTBAAU2SOBU.
   </details>

5. <details>
   <summary>What happens if two banks in the Swift network do not have a direct relationship?</summary>
   An intermediary is found who has a relationship with both banks to facilitate the transaction.
   </details>

6. <details>
   <summary>How do banks earn money within the Swift network?</summary>
   Banks earn money via the spread and/or charging fees to customers, though this process is described as expensive and inefficient.
   </details>

7. <details>
   <summary>Name three regulated online payment systems mentioned in the lecture.</summary>
   Paypal, Alipay, and Wechat.
   </details>

8. <details>
   <summary>Approximately how many internet, mobile internet, and social media users are there, according to the lecture?</summary>
   Around 4.6+ billion internet users, 4.3+ billion mobile internet users, and 4.2+ billion social media users.
   </details>

9. <details>
   <summary>How has technology impacted unbanked areas or situations where usual financial channels have failed?</summary>
   Technology has reached where banks don’t, having an impact in situations such as providing protection from loan sharks.
   </details>

10. <details>
    <summary>What are the targeted improvements for central payment systems by 2027?</summary>
    % of cross-border wholesale payments are to be credited within one hour of payment initiation, all financial institutions should have at least one option for cross-border wholesale payments, and the global average cost of payment should be no more than 1%.
    </details>

# How Cryptocurrencies work and the technology behind them
1. <details><summary>What is Cryptography and what role did it play in WWII?</summary>
   Cryptography originated from the Greek word "Kryptós," meaning "hidden" or "secret." It involves techniques to keep secrets and share them only with select parties. During WWII, cryptography played a key role, with notable contributions from Alan Turing in breaking the “Enigma” machine.
   </details>

2. <details><summary>What is Public-key (asymmetric) cryptography, and how does it work?</summary>
   Public-key cryptography uses a pair of keys: a public key and a private key. The private key should be kept secret, while the public key can be shared. It is computationally infeasible to derive the private key from the public key. Public-key cryptography is used for encryption and digital signatures.
   </details>

3. <details><summary>How does encryption work in Public-key cryptography?</summary>
   In Public-key cryptography, encryption is performed using the recipient's public key, and decryption is done using the recipient's private key. This ensures that only the intended recipient can decrypt and read the message.
   </details>

4. <details><summary>What is a digital signature and how does it work?</summary>
   A digital signature is a cryptographic technique that verifies the origin and integrity of a digital message. It is generated using the sender's private key and can be verified by anyone using the sender's public key.
   </details>

5. <details><summary>How does hashing contribute to cryptographic systems?</summary>
   Hashing is a process of converting an input of arbitrary size to a fixed size using a one-way function. It is crucial for creating tamper-proof messages and is commonly used for storing passwords securely.
   </details>

6. <details><summary>What are the ideal properties of a cryptographic hash function?</summary>
   A cryptographic hash function should be deterministic, easy to compute, sensitive to input changes, collision-resistant (low probability of different inputs producing the same output), and have a fixed output size.
   </details>

7. <details><summary>What is the significance of addresses in cryptocurrency systems?</summary>
   Addresses in cryptocurrency systems represent accounts and consist of a private key (kept secret) and a public address (shared publicly to receive funds). The ownership of an account is established through the use of private keys, public addresses, and signatures.
   </details>

8. <details><summary>How is an account’s public address generated in a cryptocurrency system?</summary>
   A public address is generated from a private key using cryptographic functions, including “trap-door” functions which are easy to compute in one direction (private key to public address) but computationally infeasible in the reverse direction.
   </details>

9. <details><summary>What is the difference between centralized and decentralized systems?</summary>
   In centralized systems, a central authority maintains the ledger, verifies identities, and prevents double spending. In decentralized systems, authority and ledger maintenance are distributed, identities are anonymous, and consensus rules prevent double spending.
   </details>

10. <details><summary>How is double spending prevented in centralized and decentralized systems?</summary>
    Centralized systems rely on a central authority to prevent double spending, while decentralized systems use consensus rules and a distributed ledger to prevent double spending.
    </details>

11. <details><summary>What vulnerabilities exist in centralized systems?</summary>
    In centralized systems, if the system is compromised (e.g., credit card information is leaked), individuals can be put at risk. The central authority is a single point of failure.
    </details>

12. <details><summary>What are the benefits and challenges of decentralized systems?</summary>
    Decentralized systems are resilient to attacks and do not have a single point of failure. However, identities are anonymous, which can make it challenging to keep bad actors out. Consensus rules are necessary to maintain integrity and prevent double spending.
    </details>

13. <details><summary>How does the blockchain contribute to decentralized systems?</summary>
    The blockchain acts as a public ledger in decentralized systems, maintaining a secure and tamper-proof record of all transactions. It enables decentralized consensus and trust without the need for a central authority.
    </details>

14. <details><summary>What role does mining and consensus play in cryptocurrency systems?</summary>
    Mining is the process of validating and securing transactions on the blockchain, while consensus mechanisms ensure that all participants in the network agree on the validity of transactions. Together, they maintain the integrity and security of the cryptocurrency system.
    </details>

15. <details><summary>What are the differences between decimal and hexadecimal numbering systems?</summary>
    The decimal numbering system is base 10, using digits 0-9. The hexadecimal numbering system is base 16, using digits 0-9 </details>

16. <details><summary>What are the required properties of cryptocurrency transactions?</summary>
    Cryptocurrency transactions must ensure completeness of instruction, authorization, non-repudiation, and be tamper-proof.
    </details>

17. <details><summary>How do digital signatures and hashing contribute to the security of transactions?</summary>
    Digital signatures and hashing provide authorization, non-repudiation, and tamper-proofing for transactions, ensuring that the sender is the owner of the account, the sender cannot deny sending the transaction, and no one has modified the transaction after it was signed.
    </details>

18. <details><summary>What are the smallest units of Bitcoin and Ethereum, and how do they relate to their respective main units?</summary>
    The smallest unit of Bitcoin is Satoshi (Sat), with 1 BTC = 10^8 Sat. For Ethereum, the smallest unit is Wei, with 1 ETH = 10^18 Wei.
    </details>

19. <details><summary>What is the general process of a cryptocurrency transaction?</summary>
    The process includes getting the public address of the receiver, creating a transaction message, signing the transaction with the sender’s private key, and sending the transaction to the network.
    </details>

20. <details><summary>What is a Bitcoin transaction and how is it structured?</summary>
    A Bitcoin transaction has one or more inputs (debits), one or more outputs (credits), and a signature. The transaction fee is calculated as the sum of inputs minus the sum of outputs.
    </details>

21. <details><summary>What are Unspent Transaction Outputs (UTXO) in Bitcoin, and why are they important?</summary>
    UTXO are unused outputs and represent indivisible units of currency. They are tracked separately to avoid double spending.
    </details>

22. <details><summary>How are Ethereum transactions different from Bitcoin transactions?</summary>
    Ethereum transactions include a recipient address, value of currency, optional data, nonce, and gas price and limit. They support more complex operations, including smart contracts.
    </details>

23. <details><summary>What is a nonce in Ethereum transactions, and why is it important?</summary>
    The nonce is a count of transactions sent from a given address, ensuring the order of transactions and preventing replay attacks.
    </details>

24. <details><summary>What are the components of a public blockchain?</summary>
    A public blockchain includes a peer-to-peer network, a set of rules for valid transactions, secured blocks as a ledger, a consensus algorithm for decentralized control, and an incentives scheme for maintenance and security.
    </details>

25. <details><summary>What is the structure of a block in a blockchain?</summary>
    A block includes a header (with previous block reference, mining details, and a merkle tree root) and a list of verified transactions.
    </details>

26. <details><summary>What is the genesis block in a blockchain?</summary>
    The genesis block is the first block in a blockchain.
    </details>

27. <details><summary>How often are new blocks created in Bitcoin, and what are their size limitations?</summary>
    In Bitcoin, a new block is created on average every 10 minutes, with a size limit of 4MB.
    </details>

28. <details><summary>How does Ethereum limit the size of blocks?</summary>
    Ethereum limits block size through gas, with limitations on the gas price and gas limit.
    </details>

29. <details><summary>How can a block in a blockchain be identified?</summary>
    A block can be identified by the hash of its header or by its height in the blockchain.
    </details>

30. <details><summary>Can everyone view blocks and transactions in a public blockchain?</summary>
    Yes, everyone can view blocks and transactions in a public blockchain using blockchain explorers.
    </details>

# Trust in Cryptocurrencies
1. <details><summary>What is the primary purpose of mining in cryptocurrencies?</summary>The primary purpose of mining in cryptocurrencies is to decentralize trust and security, rather than to create new coins. It serves as an incentive mechanism to encourage participation in the network's validation and security processes.</details>

2. <details><summary>What incentives are provided to miners in a cryptocurrency network?</summary>Miners in a cryptocurrency network are incentivized through the creation of new coins with each newly mined block and the transaction fees from transactions included in the new block.</details>

3. <details><summary>How does the rate of new Bitcoin creation change over time?</summary>The number of new bitcoins created is halved every 210,000 blocks, approximately every four years, resulting in a deflationary currency. This process started with 50 Bitcoins per block in 2009, and it is expected that no new Bitcoins will be issued after around the year 2140, with a maximum limit of 21 million BTC.</details>

4. <details><summary>How is decentralized consensus achieved in Bitcoin's network?</summary>Decentralized consensus in Bitcoin's network is achieved through the verification of transactions by multiple nodes, the independent bundling of transactions into blocks, the mining of blocks using the Proof-of-Work algorithm, the verification of new blocks by multiple nodes, and the adherence to agreed-upon rules to resolve conflicts.</details>

5. <details><summary>What is the Proof-of-Work (PoW) algorithm, and how does it contribute to the mining process?</summary>The Proof-of-Work (PoW) algorithm requires miners to find a value that, when hashed with the transaction data, meets a specific difficulty target. This process is computationally hard and requires significant resources, ensuring security and consensus in the network. Valid blocks are verified by all full nodes in the network.</details>

6. <details><summary>How is the mining difficulty adjusted in Bitcoin's network?</summary>The mining difficulty in Bitcoin's network is adjusted dynamically to ensure that new blocks are created approximately every 10 minutes, based on the time it took to mine the previous 2,016 blocks.</details>

7. <details><summary>What happens if more than one miner finds a valid nonce for the same block?</summary>If more than one miner finds a valid nonce for the same block, the network will ultimately accept the block that belongs to the longest chain, which represents the most cumulative proof-of-work.</details>

8. <details><summary>How does the energy consumption of Bitcoin's PoW algorithm compare to other entities?</summary>The energy consumption of Bitcoin's Proof-of-Work algorithm is substantial, comparable to the energy consumption of entire countries such as Austria, and is responsible for a significant percentage of the world’s total energy consumption.</details>

9. <details><summary>What is Proof-of-Stake (PoS), and how does it differ from Proof-of-Work?</summary>Proof-of-Stake (PoS) is a consensus mechanism where the chance to mine the next block is determined by a participant's stake in the system, which could be a combination of factors like the number of owned coins and the age of the coins. Unlike Proof-of-Work, it uses less computation power and the cost for malicious attempts is intrinsic (loss of currency).</details>

10. <details><summary>What significant change did Ethereum implement in the "Merge"?</summary>In the "Merge," Ethereum transitioned from a Proof-of-Work consensus mechanism to a Proof-of-Stake mechanism, resulting in a significant reduction in energy consumption by around 99.9%.</details>

11. <details><summary>How can one participate in Ethereum's Proof-of-Stake mining process?</summary>To participate in Ethereum's Proof-of-Stake mining process, one must deposit 32 ETH. Validators are then chosen from this pool of participants to validate proposed blocks, and dishonest validators risk losing their stake.</details>

12. <details><summary>What is the structure of time in Ethereum's PoS system, and how does it affect block validation?</summary>Time in Ethereum's PoS system is divided into slots and epochs, with a slot lasting 12 seconds and an epoch comprising 32 slots. In every slot, a committee of validators is randomly chosen to validate a proposed block.</details>

13. <details><summary>What risks are associated with Ethereum's Proof-of-Stake system?</summary>While Ethereum's Proof-of-Stake system is generally secure, a 51% attack is still theoretically possible, although it is riskier and more costly due to the need for substantial economic resources to acquire the necessary stake.</details>

14. <details><summary>How does the blockchain track and manage validators in a Proof-of-Stake system?</summary>The blockchain keeps track of validators—accounts that are eligible to sign blocks. Validators take turns signing blocks, and if an invalid block is signed, the validator loses its stake.</details>

15. <details><summary>What is the role of validators in Ethereum's Proof-of-Stake consensus mechanism?</summary>Validators in Ethereum's Proof-of-Stake consensus mechanism are responsible for validating proposed blocks. They are selected based on their stake in the system, and they risk losing their stake if they validate an incorrect block. This system ensures security and consensus without the need for extensive computational work.</details>


# Security and some caveats
1. <details>
   <summary>What are the key security features of a centralized system like a bank?</summary>
   Centralized systems verify identities, control access, process transactions sequentially to prevent double spending, but are vulnerable if data is exposed.
   </details>

2. <details>
   <summary>How does a decentralized system like Bitcoin ensure security?</summary>
   Decentralized systems like Bitcoin allow potential bad actors due to no access control but prevent double spending and do not store identifiable information, relying on decentralized technology for trust.
   </details>

3. <details>
   <summary>What mechanisms prevent double spending in decentralized systems?</summary>
   Decentralized systems broadcast transactions for verification, maintain a full history, require valid and verified new blocks, and consider transactions immutable after a certain number of blocks.
   </details>

4. <details>
   <summary>What are some possible attacks on a decentralized system like Bitcoin?</summary>
   Possible attacks include theft of private keys, Sybil attacks, dusting attacks, denial of service, and Finney attacks.
   </details>

5. <details>
   <summary>What are the limitations of Bitcoin's scalability?</summary>
   Bitcoin's scalability is limited by block time and size, resulting in an average of 7 transactions per second.
   </details>

6. <details>
   <summary>Can Bitcoin handle the same transaction volume as Visa or Mastercard?</summary>
   No, Bitcoin handles around 7 transactions per second, while Visa and Mastercard handle about 2000 transactions per second.
   </details>

7. <details>
   <summary>What are some potential solutions to Bitcoin's scalability issues?</summary>
   Solutions include increasing block size, optimizing network bandwidth, and using Layer 2 systems like the Lightning Network.
   </details>

8. <details>
   <summary>How can the value of a cryptocurrency be evaluated?</summary>
   The value of a cryptocurrency should reflect its provided benefits, though this is a controversial and complex issue.
   </details>

9. <details>
   <summary>What are Warren Buffet's views on the value of cryptocurrencies?</summary>
   Warren Buffet views cryptocurrencies as having no value, predicting a bad ending for them.
   </details>

10. <details>
    <summary>How has the value of Bitcoin changed over time, and what does this indicate about its value?</summary>
    Since 2017, Bitcoin's value has consistently remained above 1,000 USD, indicating a persistent belief in its value despite differing opinions.
    </details>

