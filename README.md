# EX-02-Cross-Platform-Prompting-Evaluating-Diverse-Techniques-in-AI-Powered-Text-Summarization

## AIM
To evaluate and compare the effectiveness of prompting techniques (zero-shot, few-shot, chain-of-thought, role-based) across different AI platforms (e.g., ChatGPT, Gemini, Claude, Copilot) in a specific task: text summarization.

## Scenario:
You are part of a content curation team for an educational platform that delivers quick summaries of research papers to undergraduate students. Your task is to summarize a 500-word technical article on "The Basics of Blockchain Technology" using multiple AI platforms and prompting strategies.

Your goal is to determine which combination of prompting technique + platform provides the best summary in terms of:

Accuracy

Coherence

Simplicity

Speed

User experience

## AI Used:
1.ChatGPT

2.Claude

## Algorithm:
```
Start
 ├─ Step 1: Input Setup & Target Material Definition
 │   └─ Define source content ("The Basics of Blockchain Technology", ~500 words) & target audience (undergraduate engineering students).
 ├─ Step 2: Prompt Strategy Selection
 │   ├─ Strategy A: Basic Prompt (Direct request for key sections)
 │   ├─ Strategy B: Role Prompt (Persona: Blockchain Expert)
 │   ├─ Strategy C: Context Prompt (Target Persona: First-time learner)
 │   ├─ Strategy D: Constraint Prompt (Strict word-count & structure rules)
 │   └─ Strategy E: Output Format Prompt (Strict 7-part schema + flowchart)
 ├─ Step 3: Cross-Platform Execution
 │   ├─ Run Strategies A to E on Model A (ChatGPT / OpenAI)
 │   └─ Run Strategies A to E on Model B (Claude / Anthropic)
 ├─ Step 4: Multi-Criteria Assessment
 │   └─ Evaluate outputs across 5 dimensions: Accuracy, Coherence, Simplicity, Speed, and User Experience (UX).
 ├─ Step 5: Comparative Analysis & Synthesis
 │   └─ Identify strengths, weaknesses, and instruction-following fidelity per strategy/platform pair.
 End (Generate Comparative Table & Final Verdict)
```
## Output:

### 1.Basic Prompt
### Prompt:"Summarize the article about The Basics of Blockchain Technology in simple language. Explain its meaning, working principle, features, advantages, disadvantages, and applications."

## ChatGPT:
Blockchain is a modern digital technology used to store and manage information securely. It works as a distributed digital ledger in which information is stored in blocks, and these blocks are connected together to form a chain. Each block contains transaction details, a timestamp, and a cryptographic hash that helps maintain data security.

One of the important features of blockchain is decentralization, which means that no single organization controls the entire network. Instead, multiple computers maintain copies of the same information. Blockchain also provides transparency, security, immutability, and traceability.

When a transaction takes place, it is verified by network participants before being added to a new block. Once the block is added, changing the recorded information becomes extremely difficult. Blockchain technology is widely used in Bitcoin and other cryptocurrencies, banking, healthcare, supply chain management, and digital identity verification. It helps reduce intermediaries, improve transaction security, and increase trust between users.

## Claude:

The Basics of Blockchain Technology: Summary

Meaning: A blockchain is a digital record book (ledger) shared across many computers. Data is stored in groups called blocks, and each block is linked to the one before it, forming a chain. Once data is recorded, it is very hard to change.

Working principle:

Someone requests a transaction, such as sending money.
The transaction is sent to a network of computers called nodes.
The nodes check whether it is valid.
Valid transactions are grouped into a new block.
The block gets a unique code called a hash and is linked to the previous block.
The block is added to the chain, and every node updates its copy.

Features:

Decentralized: No single owner or central authority controls it.
Transparent: Participants can see the recorded transactions.
Immutable: Past records cannot easily be altered.
Secure: Cryptography protects the data.

Advantages:

Higher security and trust
Fewer middlemen, so lower cost
Faster and traceable record keeping
No single point of failure

Disadvantages:

High energy use in some systems (e.g., Bitcoin mining)
Slower than traditional databases when handling large volumes
Stored data is hard to correct or delete
Regulations are unclear and the technology is complex to learn

Applications: Cryptocurrency (Bitcoin, Ethereum), supply chain tracking, healthcare records, digital voting, and land registry.

------------------------------------------------------------------------------------------------------

### 2. Role Prompt
### Prompt: "Act as a blockchain technology expert and explain the 500-word article 'The Basics of Blockchain Technology' to undergraduate engineering students. Summarize the important concepts in simple language with suitable real-world examples."

## Chatgpt:

As a blockchain technology expert, blockchain can be explained as a decentralized and distributed database that records digital transactions securely. Unlike traditional databases, which are controlled by a central authority, blockchain stores information across multiple computers called nodes.

Blockchain works through a process involving transaction creation, verification, block formation, and block addition. When a user initiates a transaction, the network participants verify its validity using a consensus mechanism. After verification, the transaction is grouped with other transactions into a block. Each block contains a unique cryptographic hash and the hash of the previous block, which connects all blocks securely.

For example, Bitcoin uses blockchain technology to transfer digital currency between users without requiring a central bank. Smart contracts are another important feature that automatically executes agreements when predefined conditions are satisfied.

Blockchain offers several advantages, including improved security, transparency, reduced transaction costs, and better data management. It has applications in finance, healthcare, education, voting systems, and logistics. Therefore, blockchain is considered an important technology for developing secure and trustworthy digital systems.

## Claude: 

Blockchain Basics: An Expert Explanation for Engineering Students

Think of blockchain as a shared Google Sheet that nobody can secretly edit. Everyone holds a copy, and any new entry must be approved by the group.

Key concepts

Block: A container holding transactions, a timestamp, and a hash. Example: a page in a notebook listing today’s bank transfers.
Hash: A unique digital fingerprint of the block’s data. If even one letter changes, the fingerprint changes completely.
Chain: Each block stores the previous block’s hash. Changing an old block breaks every block after it, so tampering is easy to detect.
Node: Any computer participating in the network. Thousands of nodes keep identical copies.
Consensus mechanism: The rule nodes use to agree on what is valid. Proof of Work (Bitcoin) uses computing power. Proof of Stake (Ethereum) uses locked-up coins as a guarantee.
Smart contract: Code that runs automatically when conditions are met. Example: a vending machine. Insert the correct coin and you get the item, with no shopkeeper needed.

How it works in practice
Suppose Asha sends ₹500 to Ravi. The transaction is broadcast to the nodes and verified. It is bundled into a block, hashed, and linked to the chain. All copies update, and the transfer is permanent.

Real-world examples

Bitcoin: Peer-to-peer money without banks.
Walmart: Tracks food from farm to store to find contamination sources in seconds.
Estonia: Secures citizens’ health records.
Ethereum: Runs smart contracts for apps and tokens.

Engineering takeaway: Blockchain trades speed and storage efficiency for trust, transparency, and tamper resistance. Use it when multiple parties who don’t fully trust each other must share one reliable record.

-----------------------------------------------------------------------------------------------

### 3. Context Prompt
### Prompt:"I am an undergraduate engineering student learning blockchain technology for the first time. Summarize the article 'The Basics of Blockchain Technology' in a beginner-friendly way. Assume I have no previous knowledge of blockchain. Explain technical terms with simple examples and focus on its practical applications."

## ChatGPT:
Blockchain is a technology that allows people to store and share information securely without depending on a single central authority. To understand it easily, imagine a classroom where every student maintains a copy of the same notebook. Whenever a new transaction is recorded, all students verify the information and update their notebooks. Similarly, blockchain distributes information among multiple computers in a network.

The information is stored in blocks, and each block is connected to the previous block using cryptographic hashes. This connection makes it difficult for anyone to secretly modify previously recorded information.

Blockchain has several important components. A block stores transaction details, a node is a computer participating in the network, and a hash acts like a unique digital fingerprint. A consensus mechanism helps network participants agree on whether a transaction is valid.

Blockchain is useful in many real-world situations. In banking, it helps perform secure financial transactions. In healthcare, it can help maintain medical records. In supply chain management, it helps track products from manufacturers to customers. Bitcoin is one of the most popular examples of blockchain technology.

Overall, blockchain provides a secure, transparent, and reliable way of managing digital information.

## Claude:

Blockchain for Beginners: A First-Time Learner’s Summary

What is it?
Imagine your class keeps attendance in one notebook that only the teacher controls. If the teacher makes a mistake, or someone bribes the teacher, the record changes. Now imagine every student holds an identical copy, and any change must match what most students have. Cheating becomes almost impossible. That is the idea behind blockchain.

Technical terms explained

Term	Simple meaning	Example
Ledger	A record of transactions	A bank passbook
Block	A group of records	One page of the passbook
Chain	Blocks linked in order	Pages stitched together
Hash	A unique digital fingerprint	Like your Aadhaar number, unique to the data
Node	A computer in the network	One student holding a copy
Decentralized	No single boss	A WhatsApp group with no fixed admin deciding everything
Cryptography	Math that locks data	A padlock only the right key opens

How it works

A transaction is created.
The network checks it.
It goes into a block.
The block is locked with a hash and linked to the last block.
Everyone updates their copy.

Why it matters
It removes the need to trust a single middleman, and records become very hard to fake.

Practical applications to explore

Finance: Bitcoin, cross-border payments
Supply chain: Tracking medicines or food from source to buyer
Education: Tamper-proof degree certificates
Healthcare: Secure patient records shared between hospitals
Government: Land records and e-voting
Engineering: IoT device security and smart contracts for automated agreements

Study tip: Start by building a simple blockchain in Python (about 30 lines) to see hashing and linking work.

-----------------------------------------------------------------------------------------------------

### 4. Constraint Prompt
### Prompt: "Summarize the 500-word technical article 'The Basics of Blockchain Technology' using simple English. Keep the summary between 100 and 150 words. Use short sentences and avoid complicated technical terms. Include the definition, working principle, three important features, and two real-world applications. Do not include unnecessary information."

## ChatGPT:
Blockchain is a decentralized digital ledger technology used to record and store information securely. It maintains transaction records across multiple computers instead of depending on a single central authority. Information is stored in blocks, and each block is connected to the previous block using cryptographic hashes.

Blockchain works through transaction verification. When a transaction is initiated, network participants validate it using a consensus mechanism. After successful verification, the transaction is added to a new block. This block becomes part of the existing blockchain.

The major features of blockchain are decentralization, transparency, security, immutability, and traceability. It reduces the need for intermediaries, improves data reliability, and makes unauthorized modifications difficult.

Blockchain is widely used in cryptocurrency transactions, banking, healthcare record management, supply chain tracking, and digital identity verification.

Although blockchain provides several benefits, it also has limitations such as high energy consumption in some consensus systems, scalability challenges, and implementation costs.

Thus, blockchain is an important technology for secure digital transactions and information management.

## Claude:

Blockchain Summary

Blockchain is a digital record book shared by many computers. Data is saved in blocks. Each block is linked to the one before it. This forms a chain.

How it works: A transaction is made. Computers in the network check it. The valid transaction is added to a new block. The block joins the chain. Everyone gets the updated copy.

Three features:

Decentralized: No single person controls it.
Secure: Strong codes protect the data.
Transparent: Users can view the records.

Two uses:

Cryptocurrency: Bitcoin lets people send money without banks.
Supply chain: Companies track food and goods from farm to shop.

----------------------------------------------------------------------------------------------------

## 5. Output Format Prompt
## Prompt: "Summarize the technical article 'The Basics of Blockchain Technology' using the following structured format:
1. Title
2. Introduction – Explain blockchain in 2–3 sentences.
3. Working Principle – Explain how blockchain works in steps.
4. Key Features – List five important features.
5. Advantages – Mention four advantages.
6. Applications – Give five real-world applications.
7. Conclusion – Summarize the importance of blockchain.
Use simple English, bullet points, and a small flowchart to explain the working principle."

## ChatGPT:
Title: The Basics of Blockchain Technology
1. Introduction

Blockchain is a decentralized digital ledger that stores information in a secure and transparent manner. It allows multiple computers to maintain and share transaction records without requiring a central authority.

2. Working Principle

Blockchain operates through the following steps:
1. Transaction Initiation: A user initiates a digital transaction.
2. Transaction Verification: Network participants verify the transaction.
3. Block Creation: Verified transactions are grouped into a block.
4. Block Linking: The new block is connected to the previous block using cryptographic hashes.
5. Ledger Update: The updated blockchain is distributed across the network.
3. Important Features
- Decentralization: No single authority controls the entire network.
- Transparency: Participants can verify recorded transactions.
- Security: Cryptographic techniques protect transaction information.
- Immutability: Recorded information is difficult to modify.
- Traceability: Transactions can be tracked through the blockchain.
4. Advantages
- Provides secure digital transactions.
- Reduces dependency on intermediaries.
- Improves transparency and trust.
- Helps prevent unauthorized data modification.
- Supports reliable record management.
5. Applications
- Banking: Secure financial transactions and payments.
- Healthcare: Maintaining and sharing medical records.
- Supply Chain: Tracking products from manufacturers to customers.
- Cryptocurrency: Supporting digital currencies such as Bitcoin.
- Digital Identity: Secure management and verification of digital identities.
6. Limitations
- Some blockchain networks consume large amounts of energy.
- Transaction processing can be slow in certain networks.
- Implementation and maintenance can be expensive.
- Technical knowledge is required for development and management.
7. Conclusion

Blockchain is an emerging technology that changes how digital information is stored, verified, and shared. Its decentralized structure, security, and transparency make it useful across different industries. Despite certain limitations, blockchain has significant potential to improve future digital transactions and information management.

## Claude:

1. Title

The Basics of Blockchain Technology: A Structured Summary

2. Introduction

Blockchain is a digital ledger shared across a network of computers. Data is stored in linked blocks and protected by cryptography. Because no single party controls it, records are secure and very hard to alter.

3. Working Principle
[Transaction requested]
          ↓
[Sent to network nodes]
          ↓
[Nodes verify it (consensus)]
          ↓
[Valid transactions grouped into a block]
          ↓
[Block given a hash + previous block's hash]
          ↓
[Block added to the chain]
          ↓
[All nodes update their copy]
Step 1: A user starts a transaction.
Step 2: The network verifies it using a consensus method.
Step 3: The transaction joins a new block.
Step 4: The block is linked to the chain and shared with all nodes.
4. Key Features
Decentralization: Control is spread across many nodes.
Transparency: Transactions can be viewed by participants.
Immutability: Recorded data cannot easily be changed.
Security: Cryptographic hashing protects each block.
Traceability: Every transaction has a clear history.
5. Advantages
Greater security against fraud and hacking
Lower costs by removing intermediaries
Faster, more reliable record verification
Higher trust between parties who don’t know each other
6. Applications
Cryptocurrency: Bitcoin and Ethereum
Supply chain: Tracking goods and food safety
Healthcare: Secure sharing of patient records
Voting: Tamper-resistant digital elections
Education and legal: Verified certificates and smart contracts
7. Conclusion

Blockchain offers a secure, transparent way to store and share data without a central authority. As it matures, it can improve trust and efficiency in finance, healthcare, logistics, and government.


# Result:

## Comparison of the Five Prompting Strategies

| S.No | Prompting Strategy | Main Focus | Output Characteristics |
|:---:|---|---|---|
| 1 | Basic Prompt | General instruction | Provides a simple overview of blockchain technology. |
| 2 | Role Prompt | Expert perspective | Provides a technical explanation with real-world examples. |
| 3 | Context Prompt | Student background | Provides a beginner-friendly explanation with easy examples. |
| 4 | Constraint Prompt | Specific limitations | Produces a concise and focused summary within given requirements. |
| 5 | Output Format Prompt | Structured presentation | Organizes information using headings, bullet points, and steps. |

## Overall Conclusion

The same topic, **"The Basics of Blockchain Technology,"** produces different results depending on the prompting strategy used.

- **Basic Prompting:** Provides a general overview of blockchain technology.
- **Role Prompting:** Generates an expert-level explanation with technical details and examples.
- **Context Prompting:** Makes the explanation easier to understand for beginners and undergraduate students.
- **Constraint Prompting:** Controls the length, content, and complexity of the generated summary.
- **Output Format Prompting:** Organizes information systematically using headings, lists, and structured sections.

## ChatGPT vs. Claude

| Strategy | ChatGPT Performance | Claude Performance | Winner |
| :--- | :--- | :--- | :--- |
| **1. Basic Prompt** | Dense paragraph prose; accurate but harder to scan quickly. | Clear headings, bulleted working principles, and explicit sections. | **Claude** |
| **2. Role Expert** | Technical explanation; generic examples (Bitcoin, Smart Contracts). | Intuitive analogies (*Shared Google Sheet*, *Vending Machine*) & real cases (*Walmart*). | **Claude** |
| **3. Context / Beginner** | Classroom notebook analogy; plain language definitions. | Comparative markdown table, Aadhaar card analogy, and practical Python study tip. | **Claude** |
| **4. Constraint (100–150 w)** | Failed word limit constraint (~175 words); added unprompted sections. | Passed constraint (~125 words); strict compliance with negative rules. | **Claude** |
| **5. Output Format** | Numbered text list; failed to generate the requested flowchart element. | Exact 7-part schema matching; rendered a clean ASCII text flowchart. | **Claude** |

---

## Key Performance Summary

* **Accuracy:** **Tie** — Both platforms maintained high factual precision without hallucinations.
* **Coherence & Structure:** **Claude** — Superior use of headings, tables, bullet points, and ASCII diagrams.
* **Simplicity & Pedagogy:** **Claude** — Provided actionable analogies (*Vending Machine*, *Google Sheets*) suited for students.
* **Constraint Compliance:** **Claude** — Precise token/word count budgeting and format enforcement.
* **User Experience (UX):** **Claude** — Output required zero manual re-formatting before publishing.

---

## Conclusion

1. **Optimal Strategy:** Combining **Output Format Prompting** with **Context/Role Framing** produced the highest-quality, publication-ready educational summaries.
2. **Platform Selection:** **Claude** outperformed **ChatGPT** for structured content curation due to stricter instruction-following, better formatting capabilities (ASCII flowcharts/tables), and superior educational analogies.
