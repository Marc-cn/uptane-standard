# Scope

This Working Group standardizes Uptane, a compromise-resilient framework for securing software updates delivered to electronic control units (ECUs) in ground vehicles, including passenger vehicles, light- and heavy-duty trucks, and motorcycles.

## In Scope

* **Repository roles and metadata:** The Image and Director repositories, the Root, Targets, Snapshot and Timestamp roles, delegations, and the structure and semantics of the metadata each produces.
* **Verification workflows:** Full verification on Primary ECUs and partial verification on Secondary ECUs, including the conditions under which an update is accepted or rejected.
* **Vehicle reporting and time attestation:** The vehicle version manifest, ECU version reports, and the attestation of time relied on by verification.
* **Conformance requirements:** The server-side and in-vehicle implementation requirements an implementation must meet to be Uptane-conformant.
* **Threat model:** The attacker goals and capabilities the framework defends against, which establish the security properties of the design.

## Out of Scope

* **Physical attacks:** Manual tampering with ECUs outside the vehicle.
* **Compromise of the packaged software:** Malware embedded in an otherwise trusted package.
* **Supply chain compromise:** Build systems, version control, and packaging processes, which are addressed by complementary frameworks such as in-toto.
* **In-vehicle bus programming:** OBD or UDS programming of ECUs, and authentication of communications between ECUs.
* **Repository mirroring:** Malicious mirrors substituting packages that carry matching version numbers.
* **Implementations and transport:** Specific implementations, the network transport used to deliver metadata and images, and OEM back-end architecture.

Any changes of Scope are not retroactive.
