# Security

Few interesting articles:
- [Hardware and Security: Vulnerabilities and Solutions](https://www2.seas.gwu.edu/~simha/research/HWSecBookChapter12.pdf)
  Note: this article discuss about to secure a hardware and hardware for software security
- https://www.cybok.org/media/downloads/Hardware_Security_KA_-_draft_for_review_August_2019.pdf
- [Lateral Thinking for Trustworthy Apps](https://os.inf.tu-dresden.de/papers_ps/icdcs2017-lateral-thinking.pdf). Read this to learn how isolation is required for ensuring better software security.
- [Hardware-Based Trusted Computing Architectures for Isolation and Attestation](https://www.esat.kuleuven.be/cosic/publications/article-2750.pdf)



## Threat Analysis

### Book
- Threat Modeling Designing for Security by Adam Shostack. [source](https://moodle.ufsc.br/pluginfile.php/2377555/mod_resource/content/2/Threat%20Modeling.pdf)


## Paper

- TARA+: Controllability-aware Threat Analysis and Risk Assessment for L3 Automated Driving Systems
- An Asset to Security Modeling? Analyzing Stakeholder Collaborations Instead of Threats to Assets
- Threat Modeling for Automotive Security Analysis
- Risk-Oriented Security Engineering (Interesting reading. well-written)
- Combined automotive safety and security pattern engineering approach (Interesting reading)
- [Threat Modeling for Cloud Data Center Infrastructures](https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=921695)



### Other Resources

- https://medium.com/@informationsecurity/microsoft-threat-modeling-tools-logic-28ea9dd3b18d
- Threat modeling for drivers - https://docs.microsoft.com/en-us/windows-hardware/drivers/driversecurity/threat-modeling-for-drivers
  **Note:** It has used STRDIE model, and this can be used an example for understnading the STRIDE threat modeling. 
- [A Threat-Driven Approach to Cyber Security](https://www.lockheedmartin.com/content/dam/lockheed-martin/rms/documents/cyber/LM-White-Paper-Threat-Driven-Approach.pdf). It contains few examples for attack tree
- [Threat modeling explained: A process for anticipating cyber attacks](https://www.csoonline.com/article/3537370/threat-modeling-explained-a-process-for-anticipating-cyber-attacks.html)
- 



### Tools
- https://github.com/OVVL-HSO/OVVL-Webapp
  - Thesis: https://opus.hs-offenburg.de/frontdoor/deliver/index/docId/3339/file/Bachelorthesis_Tobias_Reski_18.02.2019.pdf
- https://github.com/OVVL-HSO/OVVL-Server
- Microsoft Threat Modeling Tool 2016


## Risk Assessment

Detailed listing of various risk analysis technique can be found [here](https://www.nr.no/~abie/RiskAnalysis.htm).

Risk Analysis Steps:
- Rsik Identification
- Risk Evaluation
- Risk Treatment

### Tools
- securiCAD - https://community.securicad.com/

### Papers
- SAHARA: A Security-Aware Hazard and Risk Analysis Method
- Integrated Safety and Security Risk Assessment Methods: A Survey of Key Characteristics and Applications (has provided a comparison of various techniques)
- https://www.itgovernance.co.uk/blog/7-steps-to-a-successful-iso-27001-risk-assessment
- https://www.enisa.europa.eu/topics/threat-risk-management/risk-management/current-risk/risk-management-inventory/rm-process/risk-treatment
- https://advisera.com/27001academy/blog/2016/05/16/4-mitigation-options-risk-treatment-according-iso-27001/
- https://advisera.com/27001academy/knowledgebase/threats-vulnerabilities/

## Operating System Security

### Windows

-[PMCAP: A Threat Model of Process Memory Data on the Windows Operating System](http://downloads.hindawi.com/journals/scn/2017/4621587.pdf)

### Linux Security

- [Linux Security](https://people.eecs.ku.edu/~saiedian/710/Lectures/Readings/12-linux-security.pdf) Lecture Notes
- [OS-level Attacks and Defenses: From Software to Hardware.](https://tuprints.ulb.tu-darmstadt.de/8482/1/gens_diss.pdf)
- [LINUX AND HYPERVISOR HARDENING — APPLYING A SECURE BY DESIGN PHILOSOPHY.](https://www.starlab.io/blog/linux-and-hypervisor-hardening-applying-a-secure-by-design-philosophy)
- [WINDOWS AND LINUX OPERATING SYSTEMS FROM A SECURITY PERSPECTIVE.](https://arxiv.org/ftp/arxiv/papers/1204/1204.0197.pdf)
- Automating threat modeling using an ontology framework. 
- [Measuring a System’s Attack Surface.](https://www.cs.cmu.edu/~wing/publications/tr04-102.pdf). Note: Read this to understand the attack surfaces in Linux OS. It has also listed various resource in Linux OS.
- [Clear Linux.](https://docs.01.org/clearlinux/latest/guides/index.html#clear-linux). Note: This is a great resource.
- [Operating System Security](https://www.ibr.cs.tu-bs.de/courses/ws1920/oss/index.html). Course at TUB
- [The Security Problem](https://www.cs.uic.edu/~jbell/CourseNotes/OperatingSystems/15_Security.html)



## Software Security

### Definitions

#### Untrusted vs. Macilious Applications
An pplication can contain implementation bugs (becomes untrusted) but the application is not controlled by the attacker. If the application is controlled by attacker, then it is called malicious.

### Well-know security problems

#### Confused deputy problem

>"In information security, the confused deputy problem is often cited as an example of why capability-based security is important. A confused deputy is a legitimate, more privileged computer program that is tricked by another program into misusing its authority on the system. It is a specific type of privilege escalation.
>
>Capability systems protect against the confused deputy problem, whereas access control list-based systems do not." --[wikipedia](https://en.wikipedia.org/wiki/Confused_deputy_problem)

### Security Measures

#### Sandboxing applications
Sandboxing is a technique that enforces a security policy on executed code. The security policy includes guards
and restrictions on memory accesses, restrictions on control flow transfers, and restrictions on instructions and combinations of instructions that can be executed. [source](https://nebelwelt.net/files/12Oakland.pdf)

- [Safe Loading - A Foundation for Secure Execution of Untrusted Programs](https://nebelwelt.net/files/12Oakland.pdf)
- [Boot with Integrity, or Don’t Boot](https://link.springer.com/chapter/10.1007/978-1-4302-6572-6_6)
- [Patterns for Secure Boot and Secure Storage in Computer Systems](https://download.hrz.tu-darmstadt.de/media/FB20/Dekanat/Publikationen/TRUST/tc_patterns-LoSaWi2010.pdf)
- [Ensuring Data Integrity in Storage: Techniques and Applications](https://www.fsl.cs.sunysb.edu/docs/integrity-storagess05/integrity.html)


### Resources
- [A Theory and Tools for Applying Sandboxes Effectively](http://www.cs.cmu.edu/~mmaass/pdfs/dissertation.pdf)
- [7 must-dos for delivering app-focused security](https://techbeacon.com/security/7-must-dos-delivering-app-focused-security)
- [10 Steps to Secure Software](https://dzone.com/articles/10-steps-to-secure-software)
- [Capability Theory by Sound Bytes](http://cap-lore.com/CapTheory/)
- [Security of Embedded Software](https://www.diva-portal.org/smash/get/diva2:1149047/FULLTEXT01.pdf)
- [Introduction to Embedded Linux Security - part 1](https://embeddedbits.org/introduction-embedded-linux-security-part-1/)
- [Introduction to Embedded Linux Security - part 2](https://embeddedbits.org/introduction-embedded-linux-security-part-2/)
- https://static.sched.com/hosted_files/ossna2020/72/introduction_embedded_linux_security.pdf
- [Software Security](https://www.cs.colorado.edu/~kena/classes/5828/s12/presentation-materials/stevensonhunteralharbikhali.pdf) By Hunter Stevenson and Khalid Alharbi (Interesting - it has covered the security testing)
- [ISO/IEC 27034:2011+ — Information technology — Security techniques](https://www.iso27001security.com/html/27034.html)
- [Six security tips for embedded systems](https://www.rutronik.com/article/detail/News/six-security-tips-for-embedded-systems/)
- [PaddyFrog: systematically detecting confused deputy vulnerability in Android applications](http://lilicoding.github.io/SA3Repo/papers/2015_wu2015paddyfrog.pdf)
- 

## Automotive Security

- [Security Analysis of Android Automotive](https://rtcl.eecs.umich.edu/rtclweb/assets/publications/2020/mert-sae-2020.pdf)

## Secure IC

### IC Supply Chain security

#### Logic locking
- [MEST Webinar: Logic Locking Research (2008 - Present)](https://www.youtube.com/watch?v=S-eTSlpCh7M)
- [https://www.esat.kuleuven.be/cosic/publications/article-2750.pdf](https://eprint.iacr.org/2019/796.pdf)
- [Provably-Secure Logic Locking: From Theory To Practice](https://acmccs.github.io/papers/p1601-yasinA.pdf)
- [Logic Locking: A Survey of Proposed Methods and Evaluation Metrics](http://www.eng.auburn.edu/~vagrawal/JETTA/FULL_ISSUE_35-3/P01_Dupuis_35-3_p273-291.pdf)
- [Trustworthy Hardware Design: Combinational Logic Locking Techniques](https://link.springer.com/book/10.1007%2F978-3-030-15334-2)

### Resources
- [DARPA Doubles Down on Chip-Level Cybersecurity](https://www.allaboutcircuits.com/news/darpa-doubles-down-on-chip-level-cybersecurity/).
  >"DARPA recognizes that hardware security is a specialized discipline mostly dominated by huge merchant semiconductor companies, such as Qualcomm, Intel, and Broadcom. Through 
  >automation, DARPA hopes to democratize the process of building chip-level security, making it an achievable goal for even the smallest of IC builders."
- [Handbook for Robustness Validation of Automotive Electrical/Electronic Modules](https://tinyurl.com/y3qvuz84)
- 

### Papers
- [Opening the Doors to Dynamic Camouflaging: Harnessing the Power of Polymorphic Devices](https://arxiv.org/pdf/1811.06012.pdf)


## Other Intersting Topics

- [TrInc: Small Trusted Hardware for Large Distributed Systems](https://www.usenix.org/legacy/events/nsdi09/tech/full_papers/levin/levin.pdf)


## Processor Security
- https://iiot-world.com/ics-security/cybersecurity/in-security-process-is-as-reliable-as-luck/
- https://www.youtube.com/watch?v=YXh2aIc9u64
- https://www.youtube.com/watch?v=ERg_1F6kimg

- http://spw20.langsec.org/papers/armor_LangSec2020.pdf
- [8/28 10:21 AM] Sahoo Durga Prasad (RBEI/ESY1)AppArmor crash course
    
- https://blog.cboltz.de/uploads/apparmor-english-2016-osc.pdf


- https://medium.com/information-and-technology/so-what-is-apparmor-64d7ae211ed
- https://blog.cboltz.de/uploads/apparmor-english-2016-osc.pdf
- https://auto.economictimes.indiatimes.com/webinars/holistic-cybersecurity-for-connected-vehicle-ecosystem/644?redirect=1
- OneFuzz - A self-hosted Fuzzing-As-A-Service platform
- https://tools.ietf.org/pdf/rfc7384.pdf
- https://wrach2019.lip6.fr/slides/trng_design_fischer.pdf
- https://www.riscure.com/uploads/2018/06/Riscure_Whitepaper_Fault_injection_on_automotive_diagnostic_protocols.pdf
https://www.slideshare.net/riscure/fault-injection-on-automotive-diagnosis-protocols
- https://arxiv.org/pdf/1805.11912.pdf
- https://www.enisa.europa.eu/topics/threat-risk-management/threats-and-trends
- https://www.cybok.org/media/downloads/Hardware_Security_KA_-_draft_for_review_August_2019.pdf
- https://www2.seas.gwu.edu/~simha/research/HWSecBookChapter12.pdf
- https://www.cs.cmu.edu/~wing/publications/tr04-102.pdf
- https://www.allaboutcircuits.com/news/darpa-doubles-down-on-chip-level-cybersecurity/
- https://www.ti.com/lit/an/slaa715/slaa715.pdf?ts=1604640733992&ref_url=https%253A%252F%252Fwww.google.com%252F
- https://www.allaboutcircuits.com/news/darpa-doubles-down-on-chip-level-cybersecurity/
- https://arxiv.org/pdf/1811.06012.pdf
- https://www.mckinsey.com/industries/automotive-and-assembly/our-insights/rethinking-car-software-and-electronics-architecture#
- https://users.encs.concordia.ca/~clark/courses/1601-6150/scribe/L04c.pdf
- https://medium.com/@alissaknight/threat-modeling-of-connected-cars-using-stride-e8184764eb0a
- https://documents.trendmicro.com/assets/white_papers/wp-driving-security-into-connected-cars.pdf
- https://www.mdpi.com/2078-2489/11/5/273
- https://dl.acm.org/doi/pdf/10.1145/3337791

- https://platypusattack.com/platypus.pdf
- https://os.inf.tu-dresden.de/papers_ps/icdcs2017-lateral-thinking.pdf
- Flodding
- https://onlinelibrary.wiley.com/doi/full/10.1002/sec.1328
- http://www-i4.informatik.rwth-aachen.de/content/teaching/lectures/sub/sikon/sikonWS0203/pdf/flood-based-ddos.pdf
- https://www.sciencedirect.com/topics/computer-science/flooding-attack
- https://www.elsevier.com/books/seven-deadliest-unified-communications-attacks/york/978-1-59749-547-9
- https://www.imperva.com/learn/ddos/ddos-attacks/

- Security As Code
- https://content.microfocus.com/build-appsec-dev-tb/deliver-security-as-code
- https://www.squash.io/intro-to-security-as-code/
- https://www.oreilly.com/library/view/devopssec/9781491971413/ch04.html
- https://www.arm.com/solutions/security
- https://developer.android.com/training/articles/security-tips
- Safe load
- https://nebelwelt.net/files/12Oakland.pdf
- https://www.itemis.com/en/yakindu/security-analyst/

- Principles of Secure Processor Architecture Design
-   https://caslab.csl.yale.edu/tutorials/host2018/host_2018_szefer_tutorial_principles_sec_arch_20181115.pdf

