# CS305 Software Security
## Artemis Financial
Artemis Financial is a consulting company that develops individualized financial plans for their customers. Their focus includes savings, retirement, investments, and insurance plans. Compromise of financial data or violations of standards and laws could lead to federal, state, and international penalties, as well as damage to their reputation. Artemis Financial has recognized the need for secure applications and is therefore motivated to modernize their applications and protect their organization from external threats.

## Importance of coding securely
According to Contrast Security (2014), during the period of 2012 – 2014, “the use of open-source software has more than doubled from 6 billion to 13 billion component downloads per year”. Furthermore, “eighty percent of the code in today’s applications come from libraries and frameworks, but the risk of vulnerabilities in these components is widely ignored and {underappreciated}” (Contrast Security, 2014). The importance of coding securely is important because software applications are the predominate way that business is conducted today, and there are countless vulnerabilities to protect against.

I think I did very well at identifying vulnerabilities in the application during the code review and the static analysis. During the code review, I found a lot of code that could be exploited and cause vulnerabilities. When reviewing resources like OWASP, the VAPFD, and Oracle coding practices I found a lot of problems with the code. The static analysis was very interesting because I learned the vulnerabilities with the dependencies and how to fix them.  Performing manual code reviews and static analysis adds value to a company like Artemis Financial because it leads to a more secure application.

## The Vulnerability Assessment Process Flow Diagram (VAPFD)
The VAPFD is a guide for conducting an architectural review of the application and for reviewing the code for possible security vulnerabilities. It consists of two layers, with seven areas of concern in each layer. Each area of concern is basically a way to categorize common security concerns into manageable groups to help make the review process standardized and consistent. Using this VAPFD in conjunction with Artemis Financials’ development lifecycle is a part of an overall strategy for implementing their Secure Software Development Lifecycle (SSDLC). Overall, I found the VAPFD a great resource because it helped me focus my thoughts in specific areas where we need to address security.

## Layers of security
Information systems are exposed to countless threats, risks, and vulnerabilities. It is not possible to completely secure an application using only one product, or only one defensive measure. Implementing defense in depth at various layers of an information system requires multiple tools and resources. This might include layers such as: external network, network perimeter, internal network, host, application, and data layers. Furthermore, at each layer we will have multiple defense measures in place to protect against various vulnerabilities that the system might be exposed to. These measures include access control, encryption, data validation, vulnerability testing using static and dynamic analysis tools, manual code reviews, and many more.
## Function and security of the application
Performing static analysis and a manual code review were the primary ways I made certain the code and software application was secure. I used the OWASP Dependency Checker to perform the static analysis. This exposed the vulnerabilities in the dependencies used in the application in an automated way. To perform analysis of every dependency manually would be extremely difficult and time consuming. The code review is a manual process and is mainly based on coding experience and following guidance from industry standards and secure coding practices used throughout the industry. After I refactored the application, I verified security again using the Dependency Checker and performing another manual code review.

## Resources and tools
I used the following tools and resources for this application:
•	SonaType (mainly for their OSS Index of known vulnerabilities)
•	Automation with Maven and OWASP Dependency checker
•	OWASP website including their numerous security quick reference guides
•	CVE database by Mitre
•	The NIST vulnerability database
•	The VAPFD
•	Oracle’s Secure Coding Guidelines

The benefit of these resources is amazing, and I will continue to reference them in my future assignments and in my career as a software developer.

## Assignment highlights
There are numerous aspects of this application that should be highlighted. First, the use of automation is vital for testing and security. This application was built using Spring Boot and Maven, which enables quickly getting a project off the ground and into development. Integrating a static analysis tool like OWASP Dependency Checker was seamless. Dependency Checker provides an automated way of testing our dependencies for vulnerabilities. This is a tool that can fit easily into a secure SDLC (SSDLC) so that security is verified throughout the development of a project. Second, I think it is important to showcase how we secured the application. I implemented hashing, which can be used to verify integrity of files, passwords, etc. I also implemented a self-signed digital certificate that is used to create secure connection (SSL/TLS) through web connection (HTTPS), as well as used for the encryption and decryption of data.


