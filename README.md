# CS 305: Artemis Financial Vulnerability Assessment

### 1. Briefly summarize your client, Artemis Financial, and its software requirements. Who was the client? What issue did the company want you to address?

Artemis Financial is a financial services company that works with savings, retirement, investments, and insurance. The company wanted to improve the security of its application as part of modernizing its software. My responsibility was to review the Java application and identify vulnerabilities that could put customer information at risk. This included looking at how the application handles data, communicates through its REST API, and uses third-party dependencies.

### 2. What did you do well when you found your client’s software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall well-being?

I think I did well looking at the application from different angles instead of focusing on only one area. During my manual review, I identified issues like hard-coded database credentials, unnecessary root database access, missing authentication on endpoints, and problems with input validation. I also used OWASP Dependency-Check, which identified 293 vulnerability findings across the application's dependencies. Secure coding is important because even small mistakes can lead to unauthorized access or exposed information. For a financial company, keeping customer information protected is important for maintaining trust, preventing financial losses, and protecting the company's reputation.

### 3. Which part of the vulnerability assessment was challenging or helpful to you?

One of the more challenging parts was working through the dependency scan results because there were so many findings to review. It took some time to understand which vulnerabilities were the most serious and what needed to be addressed first. The manual code review was especially helpful because I could see how specific coding decisions created security problems. It also helped me connect my QA experience to security because I was looking at what could go wrong with the application, but from the perspective of someone intentionally trying to take advantage of a weakness.

### 4. How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?

For this project, I developed a mitigation plan that recommended adding multiple layers of security rather than relying on one solution. These recommendations included removing hard-coded credentials, limiting database permissions, implementing authentication and authorization, using HTTPS to protect communication, validating user input, and updating outdated dependencies. The project focused on assessing vulnerabilities and recommending improvements rather than implementing the changes. In the future, I would continue using OWASP Dependency-Check along with manual code reviews, CVE records, and security advisories to identify vulnerabilities. I would prioritize mitigation techniques based on how serious the vulnerability is and how much damage it could cause.

### 5. How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?

Since Project One focused on the vulnerability assessment, I did not refactor the application as part of this report. Instead, I reviewed the existing code and used OWASP Dependency-Check to identify security problems that needed to be addressed. In my mitigation plan, I recommended running application tests and performing another dependency scan after making changes. This would help confirm that the application still functions correctly and that the updates did not introduce additional vulnerabilities. I would also test authentication, input validation, and database access to make sure the security improvements were working as expected.

### 6. What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?

OWASP Dependency-Check was one of the most useful tools because it showed me how many known vulnerabilities can come from older libraries. I also used manual code review to identify issues that a dependency scan would not necessarily catch, such as hard-coded credentials and missing input validation. Reviewing CVE information and security advisories helped me better understand the vulnerabilities and possible solutions. Some coding practices I would continue using are validating input, following the principle of least privilege, protecting sensitive information, and keeping dependencies updated. These are practices I can apply to future development and QA work.

### 7. Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?

I would show future employers my completed Artemis Financial Vulnerability Assessment Report because it demonstrates my ability to review application code, identify security vulnerabilities, analyze dependency scan results, and recommend improvements. It also shows how I can use my QA background when looking at software security. Before this course, I was mostly focused on whether an application worked correctly. This project helped me think more about whether the application is secure, how someone could take advantage of weaknesses, and what can be done to prevent those problems. I think that is valuable knowledge to bring into future development and testing roles.
