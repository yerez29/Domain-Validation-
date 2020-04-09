The security and stability of Internet-based applications and web ecosystem fundamentally relies on the
trustworthiness of Certificate Authorities (CAs), which ensures that these services are trusted and
communication to them is secure. The CAs vouch for the reliability of a service by issuing a digital
certificate that binds a domain name to a public key of the service. Upon receiving the request for a
certificate for domain, a CA validates that the server issuing the request owns and controls the domain for
which it requests the certificate. After a successful ownership validation, the CA issues the certificate. The
certificate contains, among others, the public key of the requesting server and the requested domain and
is signed by the private key of the CA. The server then uses this certificate to prove its identity to clients in
the Internet. The clients use the server’s public key in the certificate to establish a secure (encrypted and
authenticated) connection to the server. Therefore, it is vital to correctly verify the domain’s ownership
by the CA during the certificate issuance process, such that clients and services will communicate with
genuine site and not an impostor.

This project deals with a critical analysis of an academic article called Domain Validation ++ For MitM-Resilient PKI by researchers from Fraunhofer SIT.

In this article, the researchers present a description of an attack on the domain valiadation mechanism used to verify entity information that is trying to register as a domain owner on the Internet.
The researchers explain step by step how an attacker can bypass the validation mechanism and register as the owner of a domain that he does not own. As a result, an attacker could take advantage of this attack as a launching point for additional attacks such as fraud, theft of details, identity theft, domain hijacking and man in the middle attack.

After describing the attack, the researchers describe a defensive mechanism called Domain Validation ++, which is designed to thwart the attack and describe how it works.

In this project I conducted a critical analysis of the above article. In it, a technical analysis of the ways of attack and defense described in the article was performed, in terms of the likelihood of their feasibility in a realistic scenario and what holes and problems arise from them in the way of operation. For each of the mechanisms I detailed the relevant critical analysis.

The original article in the Domain Validation ++ For MitM-Resilient PKI.pdf file and the analysis in the Domain Validation Analysis.pdf file.
