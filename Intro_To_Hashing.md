<div align="center">

# HASHING

</div>

<div align="center">

**Hashing** is a process that transforms data into a **fixed-length string** of characters, often referred to as a **hash value** or **digest**. Unlike encryption, hashing is **one-way**—once data is hashed, it cannot be easily reversed to its original form. Hashing is commonly used for **data integrity** and **authentication**, ensuring that data has not been altered or tampered with.

</div>

---

## **Why Hashing is Important**

- **Data Integrity**: Hashing is used to ensure that data has not been altered during transmission or storage. If the hash value of data changes, it indicates that the data has been modified.
- **Password Storage**: Hashing is commonly used to securely store passwords. Instead of storing the original password, only its hash value is saved, ensuring that even if the password database is compromised, the original passwords remain safe.
- **Digital Fingerprints**: Hashing creates a unique identifier (fingerprint) for data. Even a small change in the data will result in a completely different hash value, making it useful for verifying data authenticity.

---

## **How It Works**
In hashing, an algorithm takes an input (e.g., a password or a file) and produces a fixed-length hash value. If even a small change is made to the input data, the resulting hash will be drastically different. The hash value can be used to verify the integrity of data, but it is computationally infeasible to reverse the hash back to the original input.

For example, when you enter your password on a website, the system hashes your password and compares it to the stored hash value to see if they match.

### **Example**: **SHA-256**
- **SHA-256** (Secure Hash Algorithm) is one of the most popular hashing algorithms. It is used for checking data integrity and securing passwords in various applications, such as blockchain and file verification.

---

## **Security Considerations:**
- **Collision Resistance**: A good hashing algorithm should be resistant to collisions—situations where two different inputs produce the same hash value. Weak hashing algorithms (like MD5) are vulnerable to such attacks.
- **Salting**: Adding a unique random value (called a **salt**) to the data before hashing it helps prevent **rainbow table** attacks and increases security.

---

<br>

## **In Summary:**

Hashing is a one-way process that creates a unique fixed-length value representing the original data. It is commonly used for **data integrity**, **password storage**, and **digital signatures**. **SHA-256** is a widely used hashing algorithm. While hashing is effective for verifying the integrity of data, it cannot be reversed to reveal the original data, making it an essential tool for cybersecurity.

</br>
