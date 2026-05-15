
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

Task 3: Overview 

This practical focused on assessing and understanding the security posture of an Azure environment using Microsoft Defender for Cloud. The goal was to evaluate the current state of security, identify recommendations, and understand how security monitoring operates within a cloud environment.

Onboarding a subscription into Microsoft Defender for Cloud ensures that all resources are continuously monitored for security risks. Without onboarding, security tools cannot evaluate the environment, leaving potential vulnerabilities undetected.

Even though no active recommendations are present in this environment, proper onboarding ensures that any future deployments will automatically benefit from security monitoring and recommendations.

Security Posture – Before Configuration

At the start of the assessment, the environment had no active resources monitored by Microsoft Defender for Cloud.

- Secure Score: N/A
- Assessed Resources: 0
- Security Recommendations: 0

This indicates that the environment was not generating security insights due to the absence of active workloads.

Defender for Cloud Configuration

The Microsoft Defender for Cloud setup was reviewed to verify whether the Azure subscription was onboarded for security monitoring.

The subscription was already onboarded, meaning Defender for Cloud is active and capable of assessing any resources deployed in the environment.

Security Posture – After Configuration

After reviewing the Defender setup, the environment remained unchanged in terms of recommendations and secure score.

- Secure Score: N/A
- Recommendations: None

This is expected because there are no active resources currently being assessed. However, the environment is now confirmed to be properly configured for continuous security monitoring.

Analysis of Security Recommendations

No active recommendations were present in this environment. However, in a typical Azure deployment, common recommendations include:

1. Enabling multi-factor authentication (MFA)  
2. Securing management ports (SSH/RDP)  
3. Restricting public access to storage accounts  

These recommendations are important to reduce attack surfaces and protect sensitive data.

Severity Levels in Defender for Cloud

Microsoft Defender for Cloud assigns severity levels such as Critical, High, Medium, and Low based on the potential impact and likelihood of a security risk.

High and critical vulnerabilities typically involve risks that could lead to data breaches, unauthorized access, or system compromise. Medium risks represent moderate security concerns, while low risks are usually best practice improvements.

Factors influencing severity include whether a resource is exposed to the internet, the sensitivity of the data, and how easily the vulnerability can be exploited.

This practical demonstrated the importance of understanding cloud security posture even in environments with minimal resources. It highlighted that security tools must be properly configured to provide visibility and monitoring.

Even though no active recommendations were present, the exercise showed how Microsoft Defender for Cloud would be used in a real-world environment to continuously assess and improve security.

