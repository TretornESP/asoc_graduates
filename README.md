How to validate:

1. Ask for the email (secret) and certificate id (public) of the person you are validating.
2. Perform sha256 of the email.
3. Search the csv for the last 32 characters of the email hash.
4. If it is present and the document sha256 matches, the first step of the validation is correct.
5. If you require further validation, make sure digital signature is correct inside the doc (may eventually expire)
