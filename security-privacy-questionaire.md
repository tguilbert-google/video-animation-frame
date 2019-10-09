# Video Animation Frame - Security and Privacy Questionnaire

This document answers the [W3C Security and Privacy
Questionnaire](https://www.w3.org/TR/security-privacy-questionnaire/) for the
Video Animation Frame specification.

Last Update: 2019-10-09

**2.1. What information might this feature expose to Web sites or other parties, and for what purposes is that exposure necessary?**

This feature exposes video frame metadata. This exposure is necessary to allow web applications to automatically measure performance. 

**2.2. Is this specification exposing the minimum amount of information necessary to power the feature?**

It is exposing a reasonnable, limited set of information to make the feature useful.

**2.3. How does this specification deal with personal information or personally-identifiable information or information derived thereof?**

No PII.

**2.4. How does this specification deal with sensitive information?**

No sensitive information.

**2.5. Does this specification introduce new state for an origin that persists across browsing sessions?**

No.

**2.6. What information from the underlying platform, e.g. configuration data, is exposed by this specification to an origin?
If so, is the information exposed from the underlying platform consistent across origins? This includes but is not limited to information relating to the user configuration, system information including sensors, and communication methods.**

The specificication doesn't expose any data about the platform directly. However, it could open up side-channels, from which information about the performance of the underlying platform could be measured.

**2.7. Does this specification allow an origin access to sensors on a user’s device?**

No.

**2.8. What data does this specification expose to an origin? Please also document what data is identical to data exposed by other features, in the same or different contexts.**

It exposes data about a video element and the metadata surrounding its processing (various timestamps, frame size, processing times, frame counts). 

**2.9. Does this specification enable new script execution/loading mechanisms?**

No? It uses a new callback.

**2.10. Does this specification allow an origin to access other devices?**

No.

**2.11. Does this specification allow an origin some measure of control over a user agent’s native UI?**

No.

**2.12. What temporary identifiers might this this specification create or expose to the web?**

None.

**2.13. How does this specification distinguish between behavior in first-party and third-party contexts?**

The specificiation does not distinguish between 1st and 3rd party.

**2.14. How does this specification work in the context of a user agent’s Private Browsing or "incognito" mode?**

The specification behaves in the same way.

**2.15. Does this specification have a "Security Considerations" and "Privacy Considerations" section?**

Not yet, as the specification hasn't been formally written. The feature might allow profiling of machines, by exposing accurate video decode performance metrics. There might be a need for an explanation of what kind of risk, if any, this brings about.

**2.16. Does this specification allow downgrading default security characteristics?**

No.

**2.17. What should this questionnaire have asked?**

N/A
