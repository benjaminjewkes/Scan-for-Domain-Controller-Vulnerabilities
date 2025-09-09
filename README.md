# Scan-for-Domain-Controller-Vulnerabilities

##Overview
Performed vulnerability scanning and remediation on a Windows Server domain controller (CorpDC). Used CompTIA Vulnerability Scanner to identify misconfigurations, applied fixes in Group Policy, and verified remediation by re-scanning.

##Lab Steps
1. Logged into CompTIA Vulnerability Scanner web console.
2. Added CorpDC (192.168.0.11) as a scan target.
3. Created and executed a vulnerability scan task.
4. Reviewed scan report and identified many vulnerabilities in Default Domain Policy.
5. Go to CorpDC server
6. Event log retention set not to overwrite events for system log, security log and application log.
7. DCOM Server Process Launcher service disabled
8. Task Scheduler service disabled
9. Set password policy. Minimum password length 14 characters. Minimum password age of 1 day. Password history of 24 passwords.
10. Account lockout duration set to 60 minutes.
11. Re-ran scan to confirm vulnerabilities were resolved.

##Suggested Solution / Security Considerations
-Ensure Group Policy enforces strong password policies, account lockouts, and proper audit logging.
-Regularly schedule vulnerability scans against domain controllers and critical infrastructure.
-Document remediation steps for future audits and compliance checks.
-Integrate scanning tools into patch management.

##Key Takeaways
-Practiced end-to-end vulnerability management workflow: detection → remediation → validation.
Reinforced the importance of hardening domain controllers.
-Learned how vulnerability scanning reports map to policy misconfigurations and how to resolve them.

##Screenshots
Attached
