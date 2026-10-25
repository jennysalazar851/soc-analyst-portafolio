SOC Lab 03 Brute-Force DETECTION 
1.SCENARIO:
 A security analyst receives an alert about repeated failed login attempts against a company account 
the objective is to review the authentication logs and assess whether the activity may indicate a brute-force attack 
2.EVIDENCE OBSERVED :
 |Time |Username|Source IP   |Result    |
|----- |--------|------------|----------|
|10:01 |alex    |185.XX.XX.10|Failed    |
|10:02 |alex    |185.XX.XX.10|Failed    |
|10:03 |alex    |185.XX.XX.10|Failed    |
|10:04 |alex    |185.XX.XX.10|Failed    |
|10:05 |alex    |185.XX.XX.10|Failed    |
|10:08 |alex    |185.XX.XX.10|Successful|
NOTE: the source IP is partially masked for this training exercise 
3. INVESTIGATION QUESTIONS:
 1.five failed login attempts accurred between 10:01 and 10:05 
 2.All six events involved the same username and source IP 
 3. A successful login occurred at 10:08 three minutes after the final failed attempt 
 4. the sequence may indicate may indicate a potential account compromise,but the avavilable evidence 
 does not confirm unauthorized access 
4.INITIAL ASSESSMENT:
 the repeated authentication failures followed by a successful login are suspicious and may be consistent with a brute force attempt 
 However, the activity could also result from a legitimate user entering an incorrect password several  times. addional evidence is required to distinguish between these possibilities
5.RECOMMENDED INVESTIGATION STEPS:
AS A SOC ANALYST, I WOULD :
 1.Review the source IP address:
   determine whether it is associated with the user's normal login activity or an unfamiliar location 
 2.Examine authenthication history:
   check for additional failed login attempts involving the same account or IP address 
 3.Verify the successsful login:
   whether the user recognize the login and whether the device and location are expected.
 4.Review related security logs:
   suspicious activity after the successful authentication, including privilege escalation or unusual        access to resources 
 5.Check for other affected accounts :
   determine whether the same IP address attempted to access multiple user accounts 
 6.Correlate timestamps:
   event sequence and time zone across available log sources 

6. RECOMMENDED RESPONSE :
  If additional evidence confirms unauthorized access, the security team should follow the organization's
  incident response procedures
POTENTIAL ACTIONS INCLUDE:
-Temporarily restricting the affected account if necessary
-Revoking active sessions and resetting credentials when appropriate
-Enabling or forcing multifactor authetication (MFA)
-Blocking the source IP address when justified by the investigation and organizational policy
-Preserving relevant logs for further analysis
These actions should be based on verified evidence and the organizations security procedures.

7.CONCLUSION 
The available authentication logs show five failed login attempts followed by a successful login 
from the same IP address
This pattern is consistent with suspicious authentication activity and warrants further investigation .
However, the current evidence does not conclusively establish a brute force attack or unauthorized account access.
FINAL ASSESMENT: Potential brute force activity- inconclusive pending further inestigation 

8.SKILLS DEMONDTRATED:
-Authentication log analysis 
-Identification of suspicious login pattern 
-Basic brute force attack detection 
-Evidence- based security analysis
-Incident triage and investigation 
-Security incident documentation 

9. DISCLAIMER
 This report is based on a simulated training scenario. the findings and recommendations are intended for
educational purposes and do not represent a confirmed-real world security incident 
  
    
  
 
 
