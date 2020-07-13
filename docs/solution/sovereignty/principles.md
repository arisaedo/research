notes: some background information, this paper is based on [1].

## Principles of Self-Sovereign Identity
Based on Christopher Allen's comprehensive list of properties for Self-Sovereign Identity [2]
1. Existence
2. Control
3. Access
4. Transparency
5. Persistence
6. Interoperability
7. Consent
8. Minimalization
10. Protect

Others [1]
1. Protability
2. Interoperability
3. Minimalization
4. Protection

Important: ensure `provable`

## Signatures
Legally valid signatures.
1. Safe Curves
2. Safe Keys
3. Association
4. Auditing
5. Attacks
6. Attestations

### Association
An entity is associated with a "safe" key [1].

todo: define strong/weak association class.

### Attestation
The trust in other parties attesting to the truth of a user’s claim then adds up to the trust in the user’s claim [4]

todo: research into attestation

### Attacks
1. `Whitewashing` attacks [3].
2. `Sybil` attacks.

todo: define whitewashing and sybil attacks.

## Provable Claims
Based on principles related to `Protection`, of more specifically, users right to privacy.

### Zero Knowledge Proofs
Definition, refer to [5]. Improves `minimalization` principle [1].

Also, claims then form `protable` and `interoperable` principles [1]. But, even though these claims
would be able to be shared, they are not generic.

1. format for ease of use
2. easy upgrading


### Claims
The zk claims are still missing `metadata` [1].
1. Name
2. Timestamp
3. Validity Term
4. Proof Format
5. Proof Link: strong association with link.

Claim Expectancy and Risk
1. Limited
2. Everlasting

Levels of Escalation for Audit Logs (not mutually exclusive)
1. Passive
  - claim origin
  - pure attestation
2. Intent-Based
3. Active

note: for passive, all of these blocks are under the full control of the identity owner. This is why the last signature is always produced by the identity owner as he has the final say on whether or not to include this block in his own personalized blockchain. This is due to the Self-Sovereign Identity requirements of control and access.


todo:
  - research and define claim expectancy and associate risk
  - research TrustChain
  - research IdentityChain
  - research IPv8 Attestation App

## References
[1] Quinten Stokkink, Johan Pouwelse. Deployment of a Blockchain-Based Self-Sovereign Identity. 2018. Available:
https://ieeexplore.ieee.org/stampstamp.jsp?tp=&arnumber=8726562.

[2] Christopher Allen. The path to self-sovereign identity. 2016. Available:
http://www.lifewithalacrity.com/2016/04/the-path-to-self-soverereignidentity.html.

[3] Michal Feldman, Christos Papadimitriou, John Chuang, and Ion Stoica.
Free-riding and whitewashing in peer-to-peer systems.
IEEE Journal on selected areas in communications, 24(5):1010–1019, 2006.

[4] Sarah Azouvi, Mustafa Al-Bassam, and Sarah Meiklejohn. Who am i? secure identity registration on distributed ledgers.
In Data Privacy Management, Cryptocurrencies and Blockchain Technology, pages 373–389. Springer, 2017.

[5] Oded Goldreich, Silvio Micali, and Avi Wigderson. Proofs that yield nothing but their validity and a methodology of cryptographic protocol design.
In Foundations of Computer Science, 1986., 27th Annual Symposium on, pages 174–187. IEEE, 1986
