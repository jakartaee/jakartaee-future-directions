# Jakarta EE Future Directions Meeting Summary — July 24, 2025

**Source:** Transcript file `Jakarta EE Future Directions - 20250724.docx`

## Summary

Arjan Tijms joined the Jakarta EE Future Directions Interest Group to discuss the evolution of Jakarta Security, with a focus on Jakarta EE 12. He reviewed the history of security in Java EE and Jakarta EE, noting the shift from mostly container-managed security toward more application-programmable security while preserving existing container-managed models.

## Key Discussion Points

### Jakarta Security Evolution

Arjan described how security in Java EE originally lived across specifications such as EJB and Servlet, with a strong focus on container-managed security. Over time, Jakarta EE has added more ways for applications to participate directly in authentication and authorization decisions.

### Jakarta EE 12 Security Direction

The main Jakarta EE 12 direction discussed was making authorization more consistent and easier to use. Arjan described plans to bring Jakarta Authorization, Jakarta Authentication, and Jakarta Security together more coherently under the Jakarta Security umbrella, while still preserving vendor flexibility.

### Permission Store Proposal

A key proposal is a higher-level “permission store” model. This would allow applications to programmatically add, remove, and manage permissions, reducing reliance on `web.xml` for URL-pattern constraints and making security configuration more accessible to application developers.

### JWT and MicroProfile

The group discussed JWT and MicroProfile integration. Arjan explained that work has been done to bridge MicroProfile JWT into a Jakarta Security-style authentication mechanism, but the final direction depends on broader MicroProfile-to-Jakarta discussions, including namespace and compatibility concerns.

### Authentication Mechanism Mapping

Participants asked whether Jakarta EE 12 may support declarative or programmatic mapping of authentication mechanisms to URL patterns. Arjan confirmed this is an active area of interest, including possible support for multiple authentication mechanisms, fallback behavior, and user choice among mechanisms such as OpenID, basic authentication, or social login-style flows.

### SAML Support

There was also interest in SAML support. Arjan noted that SAML is not currently on the formal roadmap, but the Jakarta Security project would welcome contributions, especially since additional authentication mechanisms require community resources.

## Action Items / Follow-Ups

- Continue refining Jakarta Security plans for Jakarta EE 12.
- Explore higher-level permission-store APIs to simplify authorization configuration.
- Continue monitoring MicroProfile JWT and broader MicroProfile-to-Jakarta discussions.
- Consider future support for URL-pattern-based authentication mechanism mapping.
- Seek community contributors for additional authentication mechanisms, including possible SAML support.
- Share future meeting topics and speaker suggestions with Neil Patterson or Michael Redlich.
