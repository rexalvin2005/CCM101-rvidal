# Mission Reflection

This laboratory helped me understand why a host-based firewall is important even when a server is already protected by a network firewall. A host-based firewall adds another layer of security directly on the server. If an attacker gets past the network perimeter, the host firewall can still restrict connections to services and ports that are not needed.

I also learned that managing open network ports is important because every exposed service can create another possible entry point for an attacker. By allowing only necessary ports, such as SSH for administration and port 8080 for the web application, an engineer can reduce the server's attack surface. Unnecessary services and ports should remain closed whenever possible.

In a real enterprise environment, leaving a database port such as 3306 for MySQL open to the public internet is dangerous. Attackers could attempt password guessing, exploit database vulnerabilities, or try to access sensitive information. A database should normally accept connections only from authorized application servers or trusted networks, with strong authentication and additional security controls.

Completing this mission changed my perspective on how easily a server can become exposed when its security settings are not configured carefully. Running an application successfully is not enough; I must also consider which users and network connections can reach it. The activity showed me that a default-deny policy and specific allow rules can help control access more carefully.

With eight cloud laboratory missions, my GitHub portfolio now represents a broader range of skills, including cloud fundamentals, containers, storage, deployment, monitoring, and security. Organizing each mission with documentation and screenshots also helps me demonstrate what I learned and how I applied it.

Overall, I became more confident using Linux commands and checking system configurations. I now understand that cloud security is an ongoing responsibility that involves limiting access, monitoring services, reviewing firewall rules, and correcting weaknesses before they cause problems. This knowledge will help me approach future cloud projects with a stronger security mindset.
