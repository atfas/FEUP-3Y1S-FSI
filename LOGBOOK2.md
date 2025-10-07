# group05 

## Team members
Afonso Saraiva: up202304461@up.pt
Daniel Marques: up202306365@up.pt
Inês Francisco: up202304726@up.pt


# CVE-2015-0310

## Identification
- **CVE Number**: CVE-2015-0310
- Adobe Flash Player (various versions) does not properly restrict discovery of memory addresses, enabling attackers to bypass the ASLR - Address Space Layout Randomization - protection mechanism, which may lead to an unspecified impact on other platforms.
- This vulnerability applies to all Windows versions as well as macOS and Linux.

## Cataloging
- The exploit was first observed in mid-January 2015. It was publicly disclosed on January 21, and Adobe issued a security advisory together with the patch on January 22.
- **Severity**: Classified high/critical - possible ASLR bypass (potential of full compromise)
- **Score**: CVSS v2: 10.0; CVSS v3.1: 9.8
- The exploit was discovered by a security researcher identified as “Kafeine”, security researcher Timo Hirvonen of F-Secure, and Yang Dingning.

## Exploit
- A Flash memory-disclosure vulnerability exposes memory layout, defeats ASLR, and can be exploited by attackers.
- Bundled into the Angler Exploit Kit and distributed via malvertising/compromised sites to automatically target vulnerable users.
- **Difficulty**: Low - a drive-by exploit that requires no user interaction beyond visiting a malicious page; the Adobe Flash Player is attacked automatically.

## Attacks
- The exploit was observed being delivered via the Angler Exploit Kit, which commonly distributed ransomware.
- Any user running Adobe Flash Player on  Windows or macOS (before version 13.0.0.262; from versions 14.0 to 16.0.0.287) and Linux (before version 11.2.202.438) could be attacked.
- Successful exploitation enables attackers to gain access to sensitive information or facilitate remote code execution.

## Fixes/Mitigations
- Adobe issued security updates via bulletin APSB15-02, correcting the issue for affected Flash versions.
- Disable or restrict Flash in browsers, or use click-to-play.
- Inspect the version of installed Flash Player and use vulnerability scanners to detect presence of vulnerable Flash.

## Sources
- https://nvd.nist.gov/vuln/detail/CVE-2015-0310
- https://www.cvedetails.com/cve/CVE-2015-0310/
- https://www.cve.org/CVERecord?id=CVE-2015-0310
- https://www.securityweek.com/adobe-patches-flash-player-vulnerability-exploited-wild/
- https://www.tenable.com/plugins/nessus/80946
- https://www.sonicwall.com/blog/latest-adobe-flash-zero-day-cve-2015-0310-jan-22-2015
