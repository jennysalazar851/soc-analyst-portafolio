SOC investigation 02:
SUSPICIOUS LOGIN ACTIVITY
1. Incident Summary :
2. multiple failed login attempts were followed by a succesful login to a user account
3. the account subsequently accessed an email application.
4. the activity  is suspicious, but unauthorized access has not been confirmed
2. EVIDENCE OBSERVED:
   1.09:14- failed login for user Maria
   2.09:15- failed login for user Maria
   3.09:16- failed login for user Maria
   4.09:18- successful login for user Maria
   5.09:19- accesss to the email application
3. INITIAL ASSESMENT:
   1.The sequence of failed login attempts followed by succesful login may indicate a potential
   account compromise .However the available logs do not establish whether the succesful login was legitimate
   or unauthorized.
4.RECOMMENDED INVESTIGATION STEPS:
  1. Review the source IP address of each login attempt.
  2. Check the geographic location and device information, if available .
  3. Compare the login activity with the user's normal behavior
  4. Verify whether the successful login was recognized by the account owner.
  5. Review email activity for  unusual actions or unauthorized changes.
5.CONCLUSION:
  The incident requires further investigation.There is insufficent evidence to confirm an account
   compromise at this stage.
6.LAB.SKILLS PRACTICED:
  1.Authentication log analysis
  2.Suspicious activity identification
  3. Evidence- based incident assessment
  4. Security incident documentation
7.ENVIRONMENT:
 This is a simulated cybersecurity training exercise. No real user accounts or systems were investigated

   
