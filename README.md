# cs305
- ### Briefly summarize your client, Artemis Financial, and its software requirements. Who was the client? What issue did the company want you to address?
Our client was Artemis Financial, who handles sensitive financial data of their customers. They needed the security of their codebase to be assessed and (potentially) improved. I was tasked with identifying vulnerabilities, identifying and assessing actual vulnerabilities vs false-flags in dependency reports, and combing through said dependencies. Finally, we refactored the code to introduce cryptography to protect data both in storage and in transit.

- ### What did you do well when you found your client’s software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall well-being?
We ran some dependency checks and identified outdated/false-flag dependencies, as well as data flows that should be encrypted. We introduced AES-256 and forced HTTPS configuration, reinforcing the database from breaches while complying with security regulations.

- ### Which part of the vulnerability assessment was challenging or helpful to you?
This was actually my most enlightening course thus far - performing the OWASP Dependency Checks and combing through the results to assess the flagged dependencies' validities was as challenging as it was rewarding. You said in one of the YouTube videos that we should NOT be script kiddies, and this course alarmed me that I was more of one that I thought, as we should consider many more things than mere functionality when creating software!

- ### How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?
We configured SSL/TLS and used SHA-256 for checksums while avoiding hard-coding sensitive or exploitable data into the code. Static dependency checks in tandem with manual code review crawls are the best way I know how to mitigate security risks thus far!

- ### How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?
For functionality, we simply refactored the codebase and ran it to make sure it was functional. Prior to refactoring, we ran a static dependency check and then compared that check to one that we ran AFTER refactoring. It was simple to determine that no new vulnerabilities were introduced, as the reports were identical.

- ### What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?
The module resources were all helpful, but the most helpful were definitely your breakdowns of things on YouTube, clarifying both some of the prompts as well as ways to approach them. The dependency checks were very eye-opening, as, to be honest, I have never used vulnerability checking tools on any of my little projects before. One of the more implicit takeaways from this course was being paranoid about introducing new vulnerablities, so attempting to refrain from adding new dependencies (especially without researching their security) was a milestone in my approach to how to think about software development!

- ### Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?
I would showcase the report I have uploaded alongside this README, as it demonstrates that I have the ability to both assess and mitigate security vulnerabilities. There were also other skills introduced into this course like implementing encryption and security configurations while (hopefully) communicating this technical work in a clear manner, which is important in collaborative, professional environments.
