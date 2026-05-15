
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


Task 2: Security Posture Configuration

Microsoft Defender for Cloud was reviewed to determine the security configuration of the Azure environment.

The subscription was already onboarded to Microsoft Defender for Cloud, indicating that the environment is connected to Defender and capable of being monitored. However, no additional Defender plans or resource-specific protections were enabled due to limitations of the environment and the absence of active resources.

As a result, the environment currently shows no assessed resources, no recommendations, and a secure score of N/A. This is expected in a minimal or lab-based environment where resources are limited.

The configuration ensures that any future resources deployed in the environment will be automatically assessed by Microsoft Defender for Cloud.


Security Status Before Configuration

Before reviewing Defender settings, the environment showed no assessed resources and no active security recommendations. The secure score was not available.


Security Status After Configuration

After reviewing and confirming Defender onboarding, the environment remains unchanged in terms of recommendations due to the lack of active resources. However, it is now confirmed that the environment is properly onboarded and ready for security monitoring as resources are added.


Importance of Security Onboarding

Onboarding a subscription into Microsoft Defender for Cloud ensures that all resources are continuously monitored for security risks. Without onboarding, security tools cannot evaluate the environment, leaving potential vulnerabilities undetected.

Even though no active recommendations are present in this environment, proper onboarding ensures that any future deployments will automatically benefit from security monitoring and recommendations.
