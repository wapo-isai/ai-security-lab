# Capital One Incident (2019): Incident Analysis

## Entry
The DOJ complaint attributes the intrusion to a misconfigured web application firewall (WAF), which gave the attacker access to the underlying data.

## Authority
The sources reviewed do not identify the specific identity or permissions the attacker used to reach the data. They point only to a configuration vulnerability as the enabling condition.

## Action
The attacker obtained a broad set of personal and financial information, including:

- Names, addresses, ZIP codes, phone numbers, email addresses, and dates of birth
- Self-reported income, credit scores, credit limits, balances, and payment history
- Transaction data and other contact information

The attacker also obtained approximately **140,000 Social Security numbers** and **80,000 bank account numbers**.

## Visibility
- **July 17:** Capital One received a disclosure from an external researcher.
- **July 19:** Capital One's investigation confirmed the incident.
- The DOJ also described a GitHub tip and the subsequent FBI investigation.

The sources do not specify which internal logs or alerts, if any, recorded the original access.

## Containment
Capital One immediately remediated the configuration vulnerability and verified that no other instances of the same weakness existed. It also expanded its routine automated scanning to check for this class of misconfiguration continuously.