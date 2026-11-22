# Paradox Packet

The Impacket suite — Python library + tools for working with network protocols (SMB, MSRPC, Kerberos, etc.).

Essential for secretsdump, psexec, wmiexec, kerberoasting, DCSync, and more.

**Upstream:** [fortra/impacket](https://github.com/fortra/impacket)

---

## Install

### Linux / Termux

```bash
pip install impacket
# or from source
git clone https://github.com/fortra/impacket.git
cd impacket
pip install .
```

Termux works great with this (pure Python).

### Windows

```powershell
pip install impacket
```

---

## Common Tools

```bash
secretsdump.py domain/user:pass@dc-ip
psexec.py domain/user:pass@target
GetUserSPNs.py domain/user:pass -dc-ip dc-ip -request
nmap + smbclient.py / wmiexec.py / dcomexec.py
```

---

## Notes

- Extremely powerful on internal networks
- Many tools require valid credentials or relay opportunities
- Pair with Responder / ntlmrelayx for full attack chains

Use only on authorized engagements.
