# Security Concepts: Encryption vs Encoding & Principle of Least Privilege

## 1. Encryption vs Encoding

### Definition

- **Encryption** transforms readable data (plaintext) into unreadable data (ciphertext) to keep it secret from unauthorized parties. 
The data can only be recovered with the correct key and algorithm. Encryption’s goal is confidentiality

- **Encoding** transforms data from one representation to another for compatibility or transport. 
It is reversible without any secret key. Encoding’s goal is data usability.

### How they work

- Encryption uses cryptographic algorithms and keys. Without the correct key, ciphertext should be infeasible to recover.  
examaple: HTTPS:browsers and servers encrypt traffic with TLS so attackers on the network cannot read it.
- Encoding uses public, documented schemes . Anyone who knows the scheme can decode the data.
example:  URL encoding special characters (`space` → `%20`) so HTTP requests remain valid.


## 2. Principle of Least Privilege (PoLP)

### Definition

- **Principle of Least Privilege** says that any user, process, or system component should have only the minimum permissions necessary to perform its tasks. 
- It applies to human accounts, services, applications, APIs, and even containers or microservices.
PoLP, reduces the attack surface i.e, if a account is compromised, the attacker can do less damage.  
Limits the impact of bugs.

