## The Software Security Framework development model. (C-Model).

## Security Enhanced SDLC: The SSDLC Methodology
###  Spotlight on How the Secure Software Development Lifecycle Enhances Web Application Security.
**Godwin S Aruga**
DevSecOps Engineer & Solution Architect.

 
 ## The Rising Tide of Web Security Threats
As digital applications continue to expand and connect users worldwide, web applications have become prime targets for cyber threats. From data breaches and unauthorized access to injection attacks and account hijacking, the need for secure development practices has never been more critical. Organizations are increasingly aware that security must be woven into the fabric of their development processes from the very beginning.

To guide secure development, several key knowledge-based standards exist. The OWASP Top 10 is a widely recognized list of the most critical security risks for web applications, such as injection, broken authentication, and sensitive data exposure. Complementing this, the SANS/CWE Top 25 emphasizes coding errors and common weaknesses that have severe consequences for application security.

Another essential resource, the Web Security Testing Guide (WSTG), produced by the OWASP project, provides a comprehensive methodology for testing the security of web applications, covering everything from information gathering to post-deployment security analysis.

However, for early-stage developers, the sheer number of frameworks, checklists, and testing methods can be overwhelming and even contradictory, with each framework emphasizing different security phases and practices.

 **Purpose of this Model**
The purpose of this Model is to present a cohesive roadmap for integrating security into the development process through a Secure Software Development Lifecycle (SSDLC). By reviewing the most impactful security standards and practices, this model aims to provide a unified, practical approach that developers and architects can follow.


 Overview of Key Security Frameworks in SDLC
1.	**OWASP Top 10:** Focuses on identifying the most critical web security risks, providing an accessible entry point to common vulnerabilities and best practices to avoid them.
2.	**SANS/CWE Top 25:** Emphasizes software vulnerabilities that have severe impacts on systems, concentrating on coding errors that can lead to critical security flaws.
3.	**OASIS Web Application Security (WAS):** Provides detailed guidelines for secure web application practices, covering aspects from architecture to deployment security controls.
4.	**Penetration Testing Execution Standard (PTES):** A methodology for performing penetration tests, detailing phases like pre-engagement, threat modeling, and vulnerability analysis, supporting security assessment in SDLC.
5.	**Web Security Testing Guide (WSTG):** Offers a step-by-step guide for testing various components of web applications, a practical tool for developers to identify and remediate vulnerabilities throughout development.

Each of these frameworks has a distinct focus, from vulnerability awareness and prevention to testing and validation. This article will provide a structured approach to leveraging these standards within an SSDLC, simplifying security integration and fostering a more secure development environment from inception to deployment. 

## The Software Security Framework development model. (C-Model).
It's often normal for developers, solution architects and Devsec professionals to differ in development environment and possibilities when it comes to what to do to have effective security framework. The C-Model Project has been in development for many years. The aim of the project is to help people understand and answer critical aspects in the development that is what, why, when, where, and how of testing web applications. The project has delivered a complete SDLC framework, not merely a simple checklist or prescription of issues that should be addressed. Readers can use this framework as a template to build their own Security based approach or to qualify other people's processes. The C-Model incorporates the combination and analysis made from common frameworks, standards and practices on security by design principles. Hence stated as a developer, solution architect and business analyst guide to deliver optimal secured software solution. 


Writing the Testing Guide has proven to be a difficult task. It was a challenge to obtain consensus and develop content that allowed people to apply the concepts described in the guide, while also enabling them to work in their own environment and culture. It was also a challenge to change the focus of web application testing from penetration testing to testing integrated in the software development life cycle.

### Measuring Security: The Economics of Insecure Software
A basic tenet of software engineering is summed up in a quote from Controlling Software Projects: Management, Measurement, and Estimates by Tom DeMarco:  **[You can't control what you can't measure.**

Security testing is no different. Unfortunately, measuring security is a notoriously difficult process.

One aspect that should be emphasized is that security measurements are about both the specific technical issues (e.g., how prevalent a certain vulnerability is) and how these issues affect the economics of software. Most technical people will at least understand the basic issues, or they may have a deeper understanding of the vulnerabilities. Sadly, few are able to translate that technical knowledge into monetary terms and quantify the potential cost of vulnerabilities to the application owner's business. Until this happens, CIOs will not be able to develop an accurate return on security investment and, subsequently, assign appropriate budgets for software security.

While estimating the cost of insecure software may appear a daunting task, there has been a significant amount of work in this direction. In 2018 the Consortium for IT Software Quality summarized:

**…the cost of poor-quality software in the US in 2018 is approximately $2.84 trillion…**

The framework described in this document encourages people to measure security throughout the entire development process. They can then relate the cost of insecure software to the impact it has on the bottom line.

**What is Testing?**
Many things need to be tested during the development life cycle of a web application, but what does testing actually mean? The Oxford Dictionary of English defines "test" as:

test (noun): a procedure intended to establish the quality, performance, or reliability of something, especially before it is taken into widespread use.

For the purposes of this document, testing is a process of comparing the state of a system or application against a set of criteria. In the security industry, people frequently test against a set of positive and negative requirements.

**Why Perform Testing?**

This document is designed to help organizations understand what comprises a testing program, and to help them identify the steps that need to be undertaken to build and operate a modern web application security testing program.

**When to Test?**
Most people today don't test software until it has already been created and is in the deployment phase of its life cycle (i.e., code has been created and instantiated into a working web application). This is an important lesson: security testing must start early in the SDLC, not just after the application has been deployed!

Companies should inspect their overall SDLC to ensure that security is an integral part of the development process. SDLCs should include security tests to ensure security is adequately covered and comprehensive.

**What to Test?**
It can be helpful to think of software development as a combination of people, process, and technology. If these are the factors that "create" software, then it is logical that these are the factors that must be tested.

An effective testing program should have components that test the following:
•	People – to ensure that there is adequate education and awareness;
•	Process – to ensure that there are adequate policies and standards and that people know how to follow these policies;
•	Technology – to ensure that the process has been effective in its implementation.

Unless a holistic approach is adopted, testing just the technical implementation of an application will not uncover management or operational vulnerabilities that could be present. By testing the people, processes, and technology, an organization can achieve a comprehensive testing program.

Denis Verdon, Head of Information Security at Fidelity National Financial, presented an excellent analogy for this misconception at the OWASP AppSec 2004 Conference in New York:

If cars were built like applications … safety tests would assume frontal impact only. Cars would not be roll tested, or tested for stability in emergency maneuvers, brake effectiveness, side impact, compatibility with guardrails, or crash site fire conditions. But cars are tested for all of these and more. If cars were built like applications are today, there would be far fewer cars on the road.


**Principles of Testing**
There are some common misconceptions when developing a testing methodology to find security bugs in software. This chapter covers some of the basic principles that professionals should take into account.

**There is No Silver Bullet**
While it is tempting to think that a security scanner or application firewall will provide many defenses against attack or identify a multitude of problems, in reality there is no silver bullet to the problem of insecure software. While tools are important, they are just one piece of the puzzle. A comprehensive, well-planned testing strategy is essential to provide thorough security validation.

**Think Strategically, Not Tactically**
Security professionals have come to realize the fallacy of the patch-and-penetrate model that was pervasive in information security during the 1990's. The patch-and-penetrate model involves fixing a vulnerability only after it has been found. This approach does not scale in a world where attackers have access to new zero-day vulnerabilities.

Vulnerability studies such as Symantec's Internet Security Threat Report have shown that with the reaction time of attackers worldwide, the typical window of vulnerability does not provide enough time for patch deployment. These statistics validate the strategic approach recommended in this testing guide: security testing must be part of a comprehensive, strategic security initiative.

There are several incorrect assumptions in the patch-and-penetrate model. Many users believe that patches interfere with normal operations or might break existing applications. It is also incorrect to assume that performing a security test once, late in the life cycle, is sufficient to address all application security issues.
 

It is essential to build security into the Software Development Life Cycle (SDLC) to prevent reoccurring security problems within an application. Developers can build security into the SDLC by developing security practices and testing procedures, not as an afterthought, but as a fundamental part of application development.
