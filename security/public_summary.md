# Security Policy Summary

**Date:** December 13, 2025
**Status:** Active

## Scope

This security policy applies to:

- The DocuLocker SaaS product (https://www.doculocker.com/)
- DocuLocker's internal systems and operations
- All software systems developed by DocuLocker for clients

## Data Storage & Encryption Policy

### Data Protection
- **Data at Rest**: All sensitive company and client data is encrypted using industry-standard AES-256 encryption or stronger
- **Data in Transit**: All data transmitted over networks is encrypted using TLS 1.3 (minimum TLS 1.2)
- **Database Security**: All databases utilize transparent data encryption for additional protection

### Data Location & Access
- Data is stored in secure cloud environments with built-in security controls
- Access to data is strictly controlled based on the principle of least privilege
- Regular reviews ensure access rights are appropriate and current
- Multi-factor authentication is required for access to sensitive systems

### Data Handling
- Sensitive production data is never transferred to testing or development environments
- Anonymized or synthetic data is used for development and testing purposes
- All data backups are encrypted and stored in secure, geographically diverse locations

## Security Monitoring & Testing Procedures

### Security Monitoring & Testing
- **Automated Monitoring**: Security monitoring systems detect and alert on potential threats across infrastructure, code, and dependencies
- **Immediate Response**: All security alerts are investigated promptly upon receipt
- **Vulnerability Management**: Regular scanning and prompt remediation of security vulnerabilities
- **Backup Testing**: Annual testing of backup and recovery procedures
- **Access Reviews**: Quarterly verification that access rights are appropriate
- **Incident Response**: Annual testing of incident response procedures

### Compliance & Standards
- We comply with all applicable privacy laws in countries where we operate
- Our practices align with GDPR requirements, which cover most international standards
- We adhere to industry best practices for data protection and security

## Security Commitments

### Third-Party Management
- Verify third-party services have encryption, 2FA, and good security practices
- Include security requirements in all employment, contractor, and vendor agreements
- Grant all personnel only the minimum access necessary for their work (employees, contractors, vendors)

### Incident Response
- A documented incident response plan is maintained
- Security incidents are addressed promptly following established procedures
- Appropriate stakeholders are notified of significant security events

### Team Security
- Security awareness is maintained through regular team discussions
- Security considerations are factored into all business decisions

---

**Document Owner**: Director

**Note**: This is a summary of our security practices. Additional details are available under appropriate confidentiality agreements as needed.