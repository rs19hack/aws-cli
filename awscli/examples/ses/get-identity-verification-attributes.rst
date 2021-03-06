**To get the Amazon SES verification status for a list of identities**

The following example uses the ``get-identity-verification-attributes`` command to retrieve the Amazon SES verification status for a list of identities::

    aws ses get-identity-verification-attributes --identities "user1@example.com" "user2@example.com"

Output::    

 {
    "VerificationAttributes": {
        "user1@example.com": {
            "VerificationStatus": "Success"
        },
        "user2@example.com": {
            "VerificationStatus": "Pending"
        }
    },
    "ResponseMetadata": {
        "RequestId": "1ce6c9b9-d482-11e2-bc12-e98118b9c6e7"
    }
 }

If you call this command with an identity that you have never submitted for verification, that identity won't appear in the output. 

For more information about verified identities, see `Verifying Email Addresses and Domains in Amazon SES`_ in the *Amazon Simple Email Service Developer Guide*.

.. _Verifying Email Addresses and Domains in Amazon SES: http://docs.aws.amazon.com/ses/latest/DeveloperGuide/verify-addresses-and-domains.html
