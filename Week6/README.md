
Task 1: Security Posture Assessment

The Microsoft Defender for Cloud secure score provides a percentage-based indication of how well an Azure environment is configured according to security best practices.

In this environment, the secure score is shown as N/A because no resources are currently being assessed by Microsoft Defender for Cloud. This indicates that either security plans are not fully enabled or there are no active resources generating security recommendations.

A secure score normally increases as security recommendations are implemented, improving the overall posture of the environment.


Active Security Recommendations

At the time of assessment, no active security recommendations were present in the environment. This is because there are no assessed resources or security plans enabled under Microsoft Defender for Cloud.

In a typical production environment, recommendations would highlight potential misconfigurations, vulnerabilities, and security gaps such as open ports, lack of encryption, or missing authentication controls.


Top 3 Security Recommendations

No recommendations were available at the time of assessment due to the absence of active resources in the environment.

However, common high-priority recommendations in a typical Azure environment include:

1. Enable multi-factor authentication (MFA)
Risk: Without MFA, user accounts are vulnerable to unauthorized access.

2. Secure management ports (SSH/RDP)
Risk: Open management ports increase exposure to brute-force attacks.

3. Restrict public access to storage accounts
Risk: Public storage access can lead to data exposure and breaches.


Why Defender for Cloud Uses Severity Levels

Microsoft Defender for Cloud assigns severity levels such as critical, high, medium, and low to security recommendations based on the potential impact and likelihood of exploitation.

Critical and high severity recommendations indicate vulnerabilities that could lead to serious consequences such as data breaches, system compromise, or loss of control over resources. Medium severity issues represent moderate risks, while low severity recommendations are generally best practice improvements.

Factors that determine severity include whether a resource is exposed to the internet, the sensitivity of the data, potential impact on security, and how easily the vulnerability can be exploited.

