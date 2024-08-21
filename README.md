# CS305

* Briefly summarize your client, Artemis Financial, and its software requirements. Who was the client? What issue did the company want you to address?  

  Artemis Financial is a consulting company which offers individualized financial services and planning. To protect its business and clients, Artemis Financial is seeking to improve the security of its web application. Some key issues that were addressed were checksum verification to validate data and dependency analysis to address known vulnerabilities in the project. 

---

* What did you do well when you found your client’s software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall well-being?

  Recognizing known vulnerabilities and refactoring code to implement error handling and input validation are important steps in securing the application. Updating dependencies helps defend against common attacks and securely coding prevents specific weaknesses in code for attackers to exploit. Error handling prevents potentially sensitive server information from being leaked from exception errors. Additionally, input validation prevents code injection which can compromise the database. Security for any company is a must, but for a financial institution it is especially important to protect the livelihood of its users as extremely sensitive information is at risk. Database leaks would also result in a loss of trust from customers and future business partners.

---

*	Which part of the vulnerability assessment was challenging or helpful to you?

    One aspect that was challenging was the implementation of the checksum function without causing build failures. Fortunately, the console of the eclipse IDE proved helpful in resolving these errors.

---

*	How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?

    There were several aspects of the project addressed to increase security. SHA-256 hashing was used to provide a layer of verification to internal Artemis financial employees to verify data. A self-signed license was also created for internal verification of the website during development. Analysis of the maven dependency check report was used to determine what dependencies of the project may have known vulnerabilities which should be updated or directly addressed. Future projects would benefit from automatic dependency checks like this and careful consideration of industry standard coding techniques.

---

*	How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?  

    For this project the maven dependency check was utilized before and after the implementation of the SHA-256 hashing function to verify the absence of additional vulnerabilities.

---

*	What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?
  
    Security should play a proactive role in the software development lifecycle in order to drive security at every step of development. Following code standards offered by organizations like OWASP would prove valuable in accomplishing this goal. Dependencies should be checked regularly in the project and ideally security would be continuously monitored through both manual and automated testing methods.

---

*	Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?
  
    This project might help illustrate my ability in identifying and mitigating security vulnerabilities. Specific code shown might be the function used to create SHA-256 hashes.
