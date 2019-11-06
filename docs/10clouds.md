# Authentication

presentation by 10clouds

## Terminology

- The user **knows** something (password, pincode)
- The user **has** something (hardware, access to email)
- The user **is** or **does** something (biometrics)

After authentication comes authorization for specific actions.

Recovery problem: The lose access to authentication methods.
This means bypassing _some_ of the authentication.
This is a possibility for an attack.
Malicious actors may attempt to circumvent authentication for their own benefit.
(Locking someone out of ones account; Get information; Get money)

## In Web

In life, an ID card is authentication. By proving it with something you have and something you are.

In web there is anonymity.
Traditionally there was a single factor: **password**.

Passwords are fine with local stuff.
Other available options:

- Email
- Phone number
- TOTP (Time-limited One Time Password)
- Physical device
- One time codes
- Offline Contact

The recovery problem is difficult.

Configurability
What do we let the users change and how de we authorize the changes:

- Confirmation from old authentication facotr
- Notifications pf any high value changes
- Time delays before changes come into effect

Usability vs security tradeoff

- What exactly can we require of users as a minimum baseline?
- Can our required security features be misused to produce issues
- how do we encourage them to make use of additional security features? (Blizzard; incentive in the form of small reward)

## Google case Multi factor Authentication

Google enforces 2FA

All mentioned factors are used.
Security Key (U2F)

Device can be configured as trusted, skipping parts of the authentication flow.

Set up as many things as you can.

### Account recovery at Google

Fairly complex, not completely public.

Takes a lot of information into account.
Familiar IP, familiar location, familiar wifi

## Case studies of attacks

Banks use authentication for transactions
Cardless withdrawal from ATM.
The scam:

- Phising for credentials
- Add a new phone device, and bank didn't require any additional authorization.
- Withdraw money through attempt
