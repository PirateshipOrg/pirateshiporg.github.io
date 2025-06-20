+++
title = "Pirateship"
url = "docs/pirateship"
description = "Basics of Pirateship"
aliases = ["/docs"]
date = "2025-06-20"

+++


Pirateship is a consensus protocol for Trusted Execution Environments (TEEs), e.g., Intel TDX and AMD SEV-SNP.
Pirateship doesn't trust TEEs blindly and recognizes that TEEs could be compromised.
It mitigates this issue by using multiple TEE platforms within the same cluster.
The consensus protocol allows two notions of confirmation: **Commit** and **Audit**.
While a transaction commits with very low latency, it may be rolled back on the off-chance a TEE has been compromised.
Audited transactions are safe against a fraction of the TEE platforms getting compromised.


- Code: https://github.com/PirateshipOrg/pirateship
- TLA+ Spec: https://github.com/PirateshipOrg/pirateship-tla

Paper will be released soon!