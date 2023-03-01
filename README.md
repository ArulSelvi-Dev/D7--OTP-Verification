# D7-OTP-Verification

### Description:
This module offers two-factor authentication (2FA) for applications that need One Time Password (OTP) Verification based on SMS. 

### Features: 
•	Generate alpha, numeric and alphanumeric OTP to Mobile numbers.<br>
•	Custom SMS template<br>
•	Configurable OTP expiry time<br>
•	Configurable OTP code length<br>
•	OTP retry options.

### Dependencies:
	Mendix modeler 9.6.15
  
### Configuration:
1.	Create an application on D7 Control panel in order to obtain the client_id and client_secret and generate auth token.
2.	Set the value of the created authentication token in the application to a constant entitled Authentication_Token.

### Implementation:
1.	Generate OTP<br>
      -Generate the One Time Password or Verifiaction Token and send to the recipient.
2.	Resend OTP<br>
      -OTP can be re-generated using the otp_id which was returned from Generate OTP endpoint.
3.	Verify OTP<br>
      -To verify the One Time Password or Verification Token sent. Once the verification done the OTP or token will expire.
4.	Get OTP Status<br>
      -To check the status (Open, Expired) of OTP.

