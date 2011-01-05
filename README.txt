procmailgen
-----------

Small program in Python that will generate a .procmailrc file for your
convenience. You must feed the program with your email address and the
path to a file containing the mailing lists that you are subscribed to
along with the folders of your inbox you want them to be delivered.

The file has the following format:

[folder1]
list1@example.com
list2@example.com

[folder2]
list3@example.com
list4@example.com


And then you run:

./procmailgen.py mailinglist-folders my@email.com

And the program will generate a .procmailrc from the templates that
are defined within it and output the .procmailrc file to stdout.

The current templates are optimised for Dovecot mailboxes and
SpamAssassin filter but you can easily change it to feet your
needs by editing them within the program file.


More info at:

https://blogs.igalia.com/clopez/?p=56
