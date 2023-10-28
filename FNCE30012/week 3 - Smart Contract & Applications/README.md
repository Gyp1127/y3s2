# A Simple Model to Evaluate Cryptocurrencies
1. <details>
    <summary>How does the lecture define the "value" of a cryptocurrency?</summary>
    The “value” of a cryptocurrency should reflect the benefits it provides, but this is a controversial issue and it's debated whether cryptocurrencies have any value at all.
    </details>
    
2. <details>
    <summary>What are the two main categories of cryptocurrencies mentioned in the lecture?</summary>
    The two main categories are pure cryptocurrencies (e.g., Bitcoin) and tokens (e.g., FNTOM, “BMM coins”).
    </details>

3. <details>
    <summary>How are transaction fees handled in cryptocurrencies according to the lecture?</summary>
    In cryptocurrencies, coins are used to pay transaction fees which cover the costs for mining and can act as stake for the validation process of transactions.
    </details>

4. <details>
    <summary>What are the key components of the demand for a cryptocurrency?</summary>
    The demand for a cryptocurrency includes transaction demand value (medium of exchange) and storage demand value (store of value).
    </details>

5. <details>
    <summary>Which theory is borrowed to understand the transaction demand for a cryptocurrency?</summary>
    The “Quantity Theory of Money” is borrowed to understand the transaction demand for a cryptocurrency.
    </details>

6. <details>
    <summary>What are the three criteria a cryptocurrency must fulfill to be appealing as a store of value?</summary>
    A cryptocurrency must be widely accepted, allow secure storage, and have a commonly believed stable supply to be appealing as a store of value.
    </details>

7. <details>
    <summary>How is the supply of a cryptocurrency determined in the long-term valuation model?</summary>
    The supply is determined by the sum of existing coins and the number of coins to be issued in the future.
    </details>

8. <details>
    <summary>How is the value per unit of a cryptocurrency calculated in the model presented?</summary>
    The value per unit is calculated as the demand divided by the supply, taking into account transaction volume, storage demand, and other factors.
    </details>

9. <details>
    <summary>Why is it challenging to pick the right parameter values for the cryptocurrency valuation model?</summary>
    Picking the right parameter values is challenging due to uncertainties and variations in transaction data, storage demand, and other factors.
    </details>

10. <details>
    <summary>How does the market's estimation of a cryptocurrency's success probability relate to its current price?</summary>
    The market's estimation of a cryptocurrency's success probability can be inferred by comparing its current price to the predicted price based on the valuation model.
    </details>

# Intro to Smart Contracts
1. <details>
   <summary>Can blockchain be used for purposes other than transferring cryptocurrencies? If so, give an example.</summary>
   Yes, blockchain can be used for purposes other than transferring cryptocurrencies. It provides an immutable distributed ledger that can store custom data, allowing for a wide range of applications beyond just cryptocurrencies.
   </details>

2. <details>
   <summary>What are the properties of blockchains that make them beneficial for storing structured data?</summary>
   The properties of blockchains that make them beneficial for storing structured data include:
   - Immutability of past blocks
   - Robustness
   - No central authority, allowing multiple entities to access the network
   - Security
   </details>

3. <details>
   <summary>What are the common components of a public blockchain?</summary>
   The common components of a public blockchain include:
   1. A peer-to-peer network that transmits and stores transactions
   2. A set of rules defining what is a valid transaction
   3. Secured blocks that provide a ledger of all past transactions
   4. A consensus algorithm for decentralized control
   5. A sound incentives scheme for maintenance and security
   </details>

4. <details>
   <summary>How can one validate a transaction on a blockchain?</summary>
   A transaction on a blockchain can be validated via pre-defined rules in smart contracts.
   </details>

5. <details>
   <summary>What does storing data on a blockchain provide, and how can privacy be maintained?</summary>
   Storing data on a blockchain provides tamper-proof timestamped data, decentralized consensus, and transparency. Privacy can be maintained by encrypting the stored data so that only authorized users can access it.
   </details>

6. <details>
   <summary>How can the integrity of large data sets be maintained on a blockchain without storing the entire data?</summary>
   The integrity of large data sets can be maintained on a blockchain by storing only the hashes of the data. Any change in the data will require a change in its hash on the blockchain, establishing a tamper-proof property.
   </details>

7. <details>
   <summary>What is the role of "Oracles" in blockchain systems?</summary>
   "Oracles" play the role of external entities that verify the correctness of data on the blockchain, especially when the custom data requires verification from outside the system.
   </details>

8. <details>
   <summary>What is a smart contract, and where does it live?</summary>
   A smart contract is a program that may update blockchain data, and it lives directly on the blockchain. It is immutable and decentralized, with multiple copies stored across the network.
   </details>

9. <details>
   <summary>Under what conditions will a smart contract execute its functions?</summary>
   A smart contract will execute its functions when the specified conditions are met, automatically triggering the agreed-upon transactions or updates.
   </details>

10. <details>
    <summary>What are the steps involved in working with a smart contract on Ethereum?</summary>
    The steps involved in working with a smart contract on Ethereum include:
    1. Writing the smart contract in a programming language like Solidity.
    2. Deploying the smart contract on the Ethereum network, giving it a public address.
    3. Users interacting with the smart contract by sending transactions to its address.
    4. The smart contract executing the required functionality on valid transactions, which may update the contract’s internal data.
    5. Optionally, the contract can be deleted, issuing a gas refund to the contract owner.
    </details>

11. <details>
    <summary>What are tokens in the context of smart contracts, and what can they represent?</summary>
    Tokens in the context of smart contracts are themselves smart contracts with defined properties. They can represent various types of assets or rights, such as utility tokens for accessing services, asset tokens for establishing ownership, or currencies.
    </details>

12. <details>
    <summary>What are some advantages of using tokens?</summary>
    Advantages of using tokens include:
    - Greater liquidity
    - Faster and cheaper transactions
    - Transparency
    - Accessibility
    </details>

13. <details>
    <summary>What needs to be trusted when working with smart contracts?</summary>
    When working with smart contracts, one needs to trust the code and the programmer. This is because software may have bugs, and incorrect implementation can lead to vulnerabilities or unintended consequences.
    </details>

14. <details>
    <summary>What was the DAO attack, and what vulnerability did it exploit?</summary>
    The DAO attack was an incident where an attacker repeatedly withdrew Ether tokens due to a reentrancy bug in a Decentralised Autonomous Organisation's smart contract. The bug was caused by two lines of code being in the wrong order, allowing the attacker to exploit the vulnerability before the balance was updated.
    </details>

15. <details>
    <summary>How can smart contracts interact with each other?</summary>
    Smart contracts can interact with each other by sending transactions or messages. A contract can trigger functions of another contract, and this interaction can be part of complex decentralized applications.
    </details>

# Applications
1. <details><summary>What is E-Estonia and why is it considered a digitally advanced society?</summary>
    E-Estonia is a northern European country known for being the most digitally advanced society, with 98% of government interactions taking place online. It has a population of around 1.3 million and was the first country to hold elections over the internet and provide e-residency. This e-residency allows non-Estonians to access Estonia's digital services, such as starting a company, accessing banks, lodging tax returns, etc.</details>

2. <details><summary>What are some of the applications and improvements brought about by E-Estonia's digital society?</summary>
    Each citizen in E-Estonia has a card that contains their private key, establishing a secure digital identity and allowing for digital signatures, which save about 20 minutes per transaction. This system is used for online banking, taxation, health records and drug prescriptions, and voting, resulting in at least 2% of GDP saved due to digital transactions, approximately 800 years of working time saved annually, 99% of healthcare prescriptions being digital, and 800,000 healthcare queries by doctors and patients each year.</details>

3. <details><summary>What is X-Road and how does it contribute to E-Estonia's digital infrastructure?</summary>
    X-Road is an internet-based decentralized system in E-Estonia that facilitates information sharing, with participating entities retaining ownership of their data. It involves around 900 participating entities (70% government and 30% private), with around 67% of queries being automated exchanges between systems. X-Road handles 500 million queries annually and is backed by a policy that prohibits requesting information already stored via X-Road.</details>

4. <details><summary>How does E-Estonia utilize blockchain technology, and what are its benefits?</summary>
    E-Estonia was the first country to have a nationwide blockchain system, which stores hashes to provide scalability and speed, detects data breaches instantly, and provides a consistent view of the data. This technology is used for various applications including e-health records, public safety, and many others, resulting in significant time savings and improved data consistency.</details>

5. <details><summary>What is trade finance and how is it related to international trade?</summary>
    Trade finance involves the use of financial products to facilitate international trade, and it is estimated that around 80 to 90% of world trade depends on trade finance. It helps resolve trust issues between importers and exporters, ensuring that payment is made upon shipment of goods.</details>

6. <details><summary>What are the drawbacks of traditional trade finance methods and how can blockchain-based solutions address these issues?</summary>
    Traditional trade finance methods are tedious, inefficient, and susceptible to fraud, with documents being checked manually and information scattered across different systems. Blockchain-based solutions can streamline the process, reducing the time for generating letters of credit, automating verification of shipping information, and enabling automatic release of payments through smart contracts.</details>

7. <details><summary>What is Decentralized Finance (DeFi) and what are its key characteristics?</summary>
    Decentralized Finance (DeFi) is a financial system that operates on blockchain, allowing users to earn interest on their cryptocurrency through smart contracts. It offers global access, transparency, interoperability, and it supports a variety of financial applications such as prediction markets, digital token exchanges, and insurance.</details>

8. <details><summary>What are stable coins and what challenges do they face?</summary>
    Stable coins are digital assets on blockchain designed to maintain a stable value with respect to a fiat currency. They can be asset-backed or algorithmic, but they face challenges in terms of regulation, implementing Anti-Money Laundering and Counter-Terrorist Financing checks, and maintaining user trust.</details>

9. <details><summary>How does Terra USD work and what is its mechanism for maintaining stability?</summary>
    Terra USD uses an algorithmic arbitrage mechanism to keep its value pegged against USD, consisting of two coins: Terra (stable) and Luna (fluctuates). The stability is maintained through a series of financial interactions between Terra and Luna, allowing users to profit from price discrepancies and thereby incentivizing the maintenance of Terra's peg to USD.</details>

10. <details><summary>What risks are associated with Terra USD and similar stablecoin systems?</summary>
    While Terra USD offers the potential for significant yields, it also carries risks, particularly if users lose trust in the system or if there are significant market fluctuations. The reliance on algorithmic arbitrage mechanisms can also lead to vulnerabilities if not properly managed.</details>

# CBDCs
1. <details>
   <summary>What are the three core features of Central Bank Digital Currencies (CBDCs)?</summary>
   CBDCs have three core features:
   - They are considered legal tender.
   - They can be converted one to one for paper currency or digital reserve.
   - They can clear and settle transactions with finality, almost instantly.
   </details>

2. <details>
   <summary>What are the different types of Central Bank Digital Currencies mentioned in the lecture?</summary>
   The lecture mentions two different types of CBDCs:
   - Wholesale CBDCs
   - Retail CBDCs
   Additionally, CBDCs can have either two-tiered or single-tiered architectures.
   </details>

