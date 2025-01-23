# Task

1. After registration, the user can log in only after confirming their email.

- add sendEmail.js
- add to userModel.js fields `verify` (whether user confirmed their email) and `verificationCode` (code for verification the user)
- add to registration controller code for verification
- send email to user for confirmation (used sendEmail.js) by link (GET request) `http://localhost:3000/api/auth/verify/${verificationCode}`
- add to login controller verification (from req.params)
- add opportunity resend verification email (route "/verify")

2. The SendGrid email service is used.
