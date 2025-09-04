
Another important technical aspect is email verification and authentication, especially if you are using a custom domain.

How does a provider such as Gmail confirm that the email has legitimately come from your organization and not someone pretending to be you?

There are a couple of security steps you can take to ensure that your emails are delivered while spoofed emails are not.

- Sender Policy Framework (SPF): You can use an SPF setting to validate that the mail server is authorized to send emails from your email domain. SPF is enabled via a `TXT` record in your domain settings. The content of that record will depend on the system you are using to send those emails.
- DomainKeys Identified Mail (DKIM): You can use DKIM to assert that the email message has not been modified in transit from the sending server to the receiving server. DKIM records are set up in your domain settings either as a `TXT` record or a `CNAME` record, depending on your provider. These records will indicate the public encryption/decryption keys.
- Domain Message Authentication, Reporting, and Conformance (DMARC): The final step, after enabling SPF and DKIM, is to set up a DMARC record. The DMARC record tells email providers what to do if an email from your domain fails SPF or DKIM, where to send delivery reports, and how often to apply the DMARC policy. A DMARC record is added as a `TXT` record to your domain settings, as `_dmarc.yourdomain.tld`.
