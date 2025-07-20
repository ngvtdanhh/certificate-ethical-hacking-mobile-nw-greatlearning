# Defense Strategies Against SQL Injection

## 1. Input Validation

- **Whitelist approach**: Only allow characters explicitly needed.
- **Reject dangerous patterns** such as `' OR 1=1 --`, `UNION SELECT`, or comments `--`.
- **Strict type checking**: Ensure input matches expected data types (e.g., numeric IDs).

## 2. Use of Prepared Statements

- **Parameterized queries**: Use `?` or named parameters instead of string concatenation.
- **Example (PHP PDO)**:
  ```php
  $stmt = $pdo->prepare("SELECT * FROM users WHERE id = :id");
  $stmt->execute(['id' => $_GET['id']]);
  ```
  ## 3. ORM Protection

- Use ORM libraries (e.g., SQLAlchemy, Hibernate) that abstract SQL queries safely.

- Avoid raw query execution with untrusted input.

## 4. Least Privilege Principle

- Ensure the database account used by the application has only minimum permissions required.

- Do not grant DROP, DELETE, or ALTER privileges unless necessary.

## 5. Web Application Firewalls (WAF)

- Deploy WAFs to detect and block known SQLi payloads.

- Use WAFs in conjunction with logging and alerting systems for better incident response.

## 6. Monitoring and Logging

- Log failed SQL queries and user input for anomaly detection.

- Integrate with SIEM for real-time monitoring.

## 7. Regular Security Testing

- Perform automated scans using tools like SQLMap or Burp Suite Pro.

- Schedule manual code reviews and penetration tests at key release milestones.

## References:

- OWASP SQL Injection Cheat Sheet

- EC-Council SQLi Prevention Guide

- NIST SP 800-53: System and Communications Protection Controls
