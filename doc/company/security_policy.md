# Security Policy

**Date:** December 13, 2025
**Applies to:** All company personnel and systems

## Shared Responsibility

Everyone in the company is responsible for security:

- Report security concerns immediately
- Protect company and client information
- Make security decisions based on risk assessment
- Approve reasonable security expenses as needed

## Security Stack (Current Implementation)

**Identity & Access Management**:
- Password manager: KeePass
- MFA: Authenticator apps and hardware keys
- SSO: Use Google Workspace login when available (e.g., "Continue with Google")
  - This provides better security through Google's strong authentication and monitoring
  - Reduces number of passwords we need to manage
  - Makes it easier to revoke access when contractors finish

**Infrastructure Security**:
- Cloud provider: AWS (with security best practices)
- Firewall: Cloudflare WAF with managed rulesets
- DDoS protection: Cloudflare's network protection
- Monitoring: CloudTrail + GuardDuty
- Network security: Private subnets, firewalls, and access controls

**Endpoint Protection**:
- Windows: Microsoft Defender + BitLocker
- macOS: XProtect + FileVault
- Linux: LUKS + ClamAV
- Browser security: Use modern browsers (Chrome, Firefox, Safari, Edge) and keep them updated

**Communication**:
- Email: Google Workspace (with 2-factor authentication enabled)
- File storage: Google Drive (encrypted by default)
- Code repositories: GitHub (with 2-factor authentication)

## What We Must Do

### 1. Protect Company Data
- **Encryption Standards**:
  - Data at rest: AES-256 encryption (or stronger)
  - Data in transit: TLS 1.3 (minimum TLS 1.2)
  - Databases: Encrypted with transparent data encryption (TDE)
- Use reputable cloud services with built-in security (Google Workspace, AWS, etc.)
- Don't store sensitive data on personal devices
- Back up important data regularly (automated where possible)
- All backups must be encrypted and stored in separate geographic locations
- **Data Environment Separation**:
  - Never transfer sensitive production data (e.g., PII) from production to staging or testing environments
  - Use anonymized or synthetic data for development and testing

### 2. Access Control
- Use unique passwords for all accounts
- **Password Requirements**:
  - Minimum 12 characters (passphrases recommended for better memorability)
  - Must include uppercase, lowercase, numbers, and special characters
  - No reuse of previous 10 passwords
  - Change every 90 days for high-risk accounts, annually for low-risk
- Enable multi-factor authentication (MFA) everywhere available (prefer TOTP over SMS)
- Don't share passwords or accounts
- Remove access for people who leave the project immediately
- Implement principle of least privilege for all access rights

### 3. Communication Security
- Use company email for business communications
- Don't send sensitive information over unencrypted channels
- Be cautious with public Wi-Fi
- **How to Send Files Securely**:
  - For documents: Use Google Drive (already encrypted) with share links instead of email attachments
  - For code: Use GitHub repositories
  - For very sensitive data: Use DocuLocker's one-time secret feature
- **When Using Public Wi-Fi**:
  - Verify websites use HTTPS (look for lock icon in browser)
  - Avoid entering sensitive information if possible
  - Consider using your phone's hotspot instead of public Wi-Fi for sensitive work

### 4. Device Security
- Keep all devices updated (OS, software, antivirus)
- **Security Hardening**:
  - Windows: Turn on BitLocker (Control Panel > BitLocker Drive Encryption)
  - Mac: Turn on FileVault (System Preferences > Security & Privacy > FileVault)
  - All devices: Set screen lock to activate after 5 minutes
  - Enable automatic updates for OS and apps
  - Install company-approved antivirus (Microsoft Defender for Windows, XProtect for Mac)
- Report lost or stolen devices immediately
- Don't install unauthorized software on work devices
- Check with director before using new software for company work

### 5. Working with Clients and Vendors
- Verify third-party services have encryption, 2FA, and good security practices
- Include security requirements in all contractor agreements
- Give vendors minimum access needed for their work

### 6. Working Across Borders
- **Service Provider Awareness**:
  - Use cloud services based in trusted jurisdictions (US, EU, etc.)
  - Check where third-party services store their data
  - Prefer services that allow data region selection
- **Communication Across Time Zones**:
  - Security incidents: notify immediately regardless of local time
  - Use Slack/email for security updates (keeps written record)
- **Legal Compliance**:
  - Be aware of data protection laws in countries where we operate
  - Following GDPR covers most requirements (it's one of the strictest standards)
  - Be careful when using services that aren't globally recognized - understand their local implications first

## Specific Actions

### Daily Security Habits
- Lock your computer when stepping away
- Think before clicking links or downloading attachments
- Report suspicious emails/links to the team immediately

### Monthly Check
- Review who has access to what (remove if not needed)
- Check for any unusual activity in accounts
- Update passwords if any security incidents occurred in the wild

### As Needed
- When bringing on new contractors: set up proper access, require MFA
- When contractors finish: revoke all access immediately
- When using new tools: ensure they meet basic security standards
- When a client specifies data residency requirements: confirm our services can meet them

## Incident Response (What to Do When Something Goes Wrong)

1. **Immediate Steps**
   - If you suspect a breach: stop what you're doing
   - Change affected passwords
   - Disconnect affected devices from the network

2. **Notify**
   - Inform the director immediately
   - Document what happened and when

3. **Contain**
   - Don't try to fix it yourself unless you're sure how
   - Preserve evidence (don't delete logs or files)

## Compliance Basics

We comply with:
- Privacy laws in countries where we operate
- Client-specific security requirements
- Industry standards for data protection

Keep records of client security requirements and how we meet them.

## Review Schedule

- Quick review every 6 months
- Full review annually or after any security incident
- Update when we start using new tools or services

---

**This is a living document.** If something doesn't make sense or needs updating, bring it up in team discussions.