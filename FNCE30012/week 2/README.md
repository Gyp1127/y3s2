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
   75% of cross-border wholesale payments are to be credited within one hour of payment initiation, all financial institutions should have at least one option for cross-border wholesale payments, and the global average cost of payment should be no more than 1%.
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
    The decimal numbering system is base 10, using digits 0-9. The hexadecimal numbering system is base 16, using digits 0-9 and

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
