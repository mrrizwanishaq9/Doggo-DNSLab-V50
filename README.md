# Doggo DNSLab V50

**Doggo DNSLab V50** is an advanced Python-based DNS lookup, analysis, and diagnostic toolkit designed for learning, troubleshooting, network administration, and authorized DNS testing.

It provides a professional terminal interface for querying different DNS record types, testing DNS resolvers, comparing response times, checking DNS health, analyzing propagation, performing reverse DNS lookups, and exporting results into useful report formats.

## 🚀 50 Features

1. A Record Lookup
2. AAAA Record Lookup
3. CNAME Lookup
4. MX Lookup
5. NS Lookup
6. TXT Lookup
7. SOA Lookup
8. PTR / Reverse DNS
9. CAA Lookup
10. SRV Lookup
11. NAPTR Lookup
12. HTTPS Record Lookup
13. SVCB Record Lookup
14. ANY Record Lookup
15. Custom Record Type
16. IPv4-Only Mode
17. IPv6-Only Mode
18. UDP DNS Queries
19. TCP DNS Queries
20. DNS-over-HTTPS
21. DNS-over-TLS
22. DNS-over-QUIC Architecture / Support-Ready Design
23. Multiple DNS Resolvers
24. Cloudflare Resolver
25. Google Resolver
26. Quad9 Resolver
27. Custom Nameserver
28. Resolver Comparison
29. Response-Time Testing
30. DNS Health Check
31. DNS Propagation Comparison
32. Reverse IPv4 Lookup
33. Reverse IPv6 Lookup
34. JSON Export
35. CSV Export
36. TXT Report Export
37. Query History
38. Local DNS Cache
39. Batch Domain Scanning
40. Batch Record Scanning
41. Domain Validation
42. IDN / Punycode Handling
43. Timeout Control
44. Retry Control
45. Color Terminal Interface
46. Debug Mode
47. Interactive Menu
48. CLI Mode
49. Configuration Save / Load
50. V50 Dashboard + DNS Diagnostics + Statistics

## 🔎 Supported DNS Records

Doggo DNSLab can work with commonly used DNS records such as:

* A
* AAAA
* CNAME
* MX
* NS
* TXT
* SOA
* PTR
* CAA
* SRV
* NAPTR
* HTTPS
* SVCB
* ANY
* Custom DNS record types

Some DNS record types may depend on the DNS server, domain configuration, or installed `dnspython` version.

## 🌐 DNS Resolver Support

The project includes support for multiple public DNS resolvers, including:

* Cloudflare — `1.1.1.1`
* Google — `8.8.8.8`
* Quad9 — `9.9.9.9`
* Custom DNS server

You can compare resolvers and measure their response times to understand how DNS resolution behaves across different servers.

## 🔐 DNS Protocol Support

Doggo DNSLab supports or provides architecture for several DNS communication methods:

* UDP DNS
* TCP DNS
* DNS-over-HTTPS (DoH)
* DNS-over-TLS (DoT)
* DNS-over-QUIC architecture / support-ready design

DoH and DoT provide encrypted DNS transport, while the DoQ component is structured as a future/support-ready architecture rather than pretending to provide a full DoQ implementation where the required protocol library is not present.

## ⚡ DNS Diagnostics

The diagnostic system can help inspect:

* DNS response time
* Resolver availability
* DNS query success/failure
* DNS health
* DNS propagation differences
* Reverse DNS
* Resolver comparison
* Timeout conditions
* Retry behavior
* Cache status
* Query statistics

Example output:

```text
✓ DNS QUERY SUCCESSFUL

Domain   : example.com
Record   : A
Resolver : 1.1.1.1
Protocol : UDP
Time     : 24.31 ms
Cached   : NO
Answers  : 1

  [01] 93.184.216.34
```

Actual DNS results, IP addresses, response times, and answer counts can change depending on the domain, resolver, network, and time of the query.

## 📦 Batch Scanning

Doggo DNSLab supports batch operations so multiple domains or record types can be processed without manually performing every query.

Example:

```text
example.com
google.com
github.com
openai.com
```

The results can then be analyzed or exported as reports.

## 💾 Cache & History

The application includes a lightweight local DNS cache and query history system.

It can keep information such as:

* Previous domains
* Record types
* Resolver used
* Query results
* Response time
* Cache status
* Query timestamps

This makes repeated DNS testing faster and easier to review.

## 📊 Export & Reporting

Results can be exported into:

* JSON
* CSV
* TXT

This makes the project useful for documentation, classroom demonstrations, troubleshooting records, and authorized network diagnostics.

## 🌍 Domain Validation

The validator accepts normal domains and can handle URL-style input.

For example:

```text
https://www.google.com
```

can be normalized to:

```text
www.google.com
```

It also provides:

* Domain validation
* ASCII representation
* Unicode representation
* Punycode / IDN handling

## 🖥️ Interactive Terminal Dashboard

V50 includes an interactive terminal interface for accessing DNS functions from a central dashboard.

The interface can provide:

```text
╔════════════════════════════════════════════════════╗
║             DOGGO DNSLAB V50                      ║
║       DNS LOOKUP & DIAGNOSTIC LAB                 ║
╚════════════════════════════════════════════════════╝

[1]  A Record
[2]  AAAA Record
[3]  Domain Validation
[4]  DNS Health Check
[5]  Resolver Comparison
[6]  Propagation Test
[7]  Reverse DNS
[8]  Batch Scanner
[9]  Export Reports
[10] Configuration
...
```

## 🧰 CLI Mode

The project can also be used from the command line without relying entirely on the interactive menu.

This makes it easier to integrate DNS testing into personal learning workflows and authorized diagnostic tasks.

## 🐍 Technology Stack

Doggo DNSLab V50 is primarily built with Python.

Main technologies include:

* Python
* `dnspython`
* `requests`
* JSON
* CSV
* Socket networking
* TLS
* DNS protocols
* Terminal UI

## 📥 Installation

Install the required Python packages:

```powershell
python -m pip install dnspython requests
```

If you are using Python 3.13 specifically:

```powershell
& "C:\Users\Dell\AppData\Local\Python\pythoncore-3.13-64\python.exe" -m pip install dnspython requests
```

Verify the DNS module:

```powershell
python -c "import dns; import dns.resolver; import dns.rdatatype; import dns.exception; import dns.query; print('DNS MODULE OK')"
```

Expected:

```text
DNS MODULE OK
```

## ▶️ Run

From VS Code terminal:

```powershell
python Doggo_DNSLab_V50.py
```

Or with Python 3.13:

```powershell
& "C:\Users\Dell\AppData\Local\Python\pythoncore-3.13-64\python.exe" "C:\Users\Dell\Desktop\pythonvs\.vscode\Doggo_DNSLab_V50.py"
```

## 🎯 Example Domains

For testing, you can enter domains such as:

```text
example.com
google.com
github.com
openai.com
youtube.com
```

You can also provide URL-style input:

```text
https://www.google.com
```

The application extracts the domain before performing DNS validation or lookup.

## 📚 Educational Purpose

Doggo DNSLab V50 is especially useful for students and developers who want to understand:

* How DNS works
* DNS record types
* Name resolution
* Recursive resolvers
* DNS transport protocols
* Resolver performance
* Reverse DNS
* DNS propagation
* Domain names and IDNs
* Network diagnostics
* Python networking

## ⚠️ Responsible Use

Use Doggo DNSLab only for domains, systems, and networks that you own or are authorized to test.

The project is intended for **education, troubleshooting, research, system administration, and authorized DNS diagnostics**. Respect DNS provider policies, network policies, and applicable laws.

## 👨‍💻 Project Goal

The goal of Doggo DNSLab V50 is to turn a simple DNS lookup utility into a complete educational DNS laboratory where users can query records, compare resolvers, perform diagnostics, test DNS behavior, save results, and understand how modern DNS systems operate.

**Doggo DNSLab V50 — Query. Analyze. Diagnose. Learn.**
