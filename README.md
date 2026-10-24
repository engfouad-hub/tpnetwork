# Atlas Industrie –- network architecture repository
Design of the Atlas Industrie network, the fictitious company of the
"Advanced Network Architectures" course. One folder per object type;
the addressing plan is authoritative in `data/vlans.yml`.
Local check: `python3 scripts/check_vlans.py` from the repository root.

## What the check does not do
`scripts/check_vlans.py` only detects duplicate VLAN IDs and overlapping
IPv4 networks. It does not validate IPv6 prefixes, mandatory fields, or
whether each VLAN sits inside its zone block.