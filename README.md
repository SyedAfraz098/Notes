📘 Serialization & Deserialization — Notes
🔹 Your Core Points (Simplified & Structured)

Scenario:
When two systems (like frontend and backend) are built using different languages or environments, they need a common way to exchange data.

Example:

Frontend → written in JavaScript

Backend → written in Java, Python, or Rust

When data is sent from frontend to server, and again from server to frontend,
both sides must follow a common serialization standard —
so that each side can parse (understand) the data correctly.
To exchange data properly, they must agree on a common data format for serialization

🔹 Definition
Serialization:
The process of converting data or objects into a common format for transmission or storage.

Deserialization:
The process of converting that common format back into usable data or objects.

🔹 Common Serialization Standards

The most common standard for client-server (HTTP) communication → JSON

Other text-based formats: XML, YAML

| Format                                                         | Type       | Common Use                                                   | Example                                           |
| -------------------------------------------------------------- | ---------- | ------------------------------------------------------------ | ------------------------------------------------- |
| **JSON (JavaScript Object Notation)**                          | Text-based | Most common for web (HTTP) communication                     | `{ "name": "Alex", "age": 25 }`                   |
| **XML (Extensible Markup Language)**                           | Text-based | Used in web services, configuration files                    | `<person><name>Alex</name><age>25</age></person>` |
| **YAML (YAML Ain’t Markup Language)**                          | Text-based | Easier to read for configs                                   | `name: Alex  age: 25`                             |
| **Binary formats (e.g., Protocol Buffers, Avro, MessagePack)** | Binary     | Faster & smaller in size (used in performance-critical apps) | (Machine-readable binary)                         |
