#  DNS Investigation Lab (Linux)

##  Overview

This project simulates and investigates DNS resolution issues in a Linux environment. The goal was to identify, analyze, and resolve DNS-related failures, including a simulated DNS spoofing scenario.

---

## Objectives

* Analyze DNS resolution failures
* Identify incorrect or malicious DNS behavior
* Compare local vs external DNS results
* Simulate DNS spoofing using the hosts file
* Apply troubleshooting techniques used in real-world SOC environments

---

##  Environment

* OS: Ubuntu Linux
* Tools: dig, nslookup, ping, resolvectl
* Editor: Visual Studio Code

---

##  Investigation Steps

### 1. Initial DNS Query

Used `dig` and `nslookup` to check domain resolution.

### 2. Connectivity Testing

Used `ping` to verify reachability.

### 3. DNS Configuration Review

Checked `/etc/resolv.conf` for DNS server settings.

### 4. External DNS Comparison

Queried Google DNS (8.8.8.8) to compare results.

### 5. DNS Spoofing Simulation

Modified `/etc/hosts` to simulate a malicious DNS override.

### 6. Issue Resolution

Removed the malicious entry and restored proper resolution.

---

## Key Findings

* Incorrect DNS resolution was caused by a local hosts file override
* System returned a false IP address (192.168.1.100)
* External DNS servers returned correct results

---

## Resolution

* Removed malicious hosts file entry
* Flushed DNS cache
* Verified correct DNS behavior

---

## Lessons Learned

* Local hosts file overrides DNS resolution completely
* Comparing DNS servers is critical for troubleshooting
* Linux tools like `dig` provide deeper insight than basic tools
* Following a structured investigation process is essential in cybersecurity

---

## Screenshots

(Add your screenshots here)

---

## Skills Demonstrated

* DNS troubleshooting
* Linux system navigation
* Network analysis
* Problem-solving in a simulated SOC scenario
* Cybersecurity investigation methodology
