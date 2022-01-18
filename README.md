# Password-manager

A *[password manager per JEVE](http://jevemanagerpsw.altervista.org)*  which, thanks to the help of multilevel access, establishes, for each user, which are the accessible and non-accessible areas.

## How it works

Privileges are managed thanks to the binary string 'accesses' (i.e 001) contained in the DB. The number of dedicated "bits" corresponds to the various reserved areas of the web application. If the digit in that position is '1' then the user will have full access to that area and vice versa.

** JEVE case:**

We have two areas and therefore two digits in our access string. The first digit represents the ability to view and modify users while the second refers to the administrator user.

* Example 1: *

* username: mariorossi@example.com
* accesses: 10

The user mariorossi@example.com will only access the first page.

* Example 2: *

* username: tiziocaio@example.com
* accesses: 11

The user tiziocaio@example.com will access all pages.




