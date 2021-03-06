Memory Hole Protected E-mail Headers
====================================

Encrypted or signed e-mail does not have cryptographic protection of
headers -- only the body of an e-mail message is encrypted or signed.

The Memory Hole project aims to fix this problem by stashing relevant
headers within the body of the e-mail in a standardized way.
Compatible mail user agents should be able to use this structure to
display the cryptographically protected headers to the user,
indicating their protection.

Messages composed using either PGP/MIME or S/MIME should be able to
use Memory Hole to add cryptographic protection for mail headers.

Things in this repository:

corpus/ -- A collection of of e-mail messages that follow the Memory
           Hole standard.  Mail user agents interested in supporting
           this technique can use this corpus as a test vector to
           verify their implementations.

specs/ -- A draft standard of how to structure and interpret these
          messages.

guidance/ -- Documentation of guidance for implementors, including
             UI/UX, deployment, and configuration considerations

screenshots/ -- Screenshots of mail user agents rendering the corpus

history/ -- Documents showing early development and documentation of
            the project.
