**Briefly summarize your client, Artemis Financial, and its software requirements. Who was the client? What issue did the company want you to address?**

Artemis Financial wanted to modernize their web application with updated security, most specifically the implementation of file verification.

**What did you do well when you found your client’s software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall well-being?**

I researched and incorporated trusted hashing algorithm SHA-256 to protect data, and incorporated secure error handling to the best of my ability.  Secure error handling is important for a company's well-being as it could divert a hacker's attention away from a possible vulnerability.

**Which part of the vulnerability assessment was challenging or helpful to you?**

The most challenging hurdle in dealing with vulnerability assessments was dealing with the slightly outdated code base with the most recent version of Java.  For this project, getting my self-signed certificate to appear as trustworthy in Google Chrome also required some researching - I tried to create a new key to include SAN in the generation, but the project wouldn't even run with the new alias...destroying the keystore and starting anew managed to check all the boxes, however.

**How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?**

Artemis Financial specifically wanted to include file verification to it's web application, which we accomplished through the use of a self-signed certificate.  This is also reflected in our use of a secure browser using HTTPS protocol and our appropriately encrypted checksum.

**How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?**

By running a Maven dependency-check on the unaltered code and comparing it to a dependency-check performed on my refactored code, it is seen that the number of vulnerabilities in the reports remained the same.  Admittedly, since it was bulleted so far down on the list, I had not run the initial dependency-check, but I still had the zip folder with the code base for the assignment.  I simply created a new, fresh project and ran the dependency-check on that.

**What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?**

A bunch of resources come to mind, namely the OWASP Dependency-Check, the class resources including the vulnerability assessment flow diagram, and the myriad of random tutorial websites I bounced around trying to get my self-signed certificate to be Chrome approved.

**Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?**

I've attached the template as well as the code because I believe the screenshots and explanation of my work reflect an understanding of the code.  The template I believe shows an appropriate understanding of the fundamentals of software security.
