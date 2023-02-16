# passwordchecker
This Python script takes a text file as an argument and will read each line as a password, compare that to the Have I Been Pwned? API 
which returns a list of 300-500 SHA1 hash suffixes that match your the first five characters in the SHA1 hash
of your own passwords that you have safely in your text file.

Now, the Have I Been Pwned? website is most likely pretty safe to trust in the first place, because the way they compare the SHA1 hash of your password
uses the same k-anonymity safety precaution as I described above. Meaning no one will be able to know for sure what your first five characters of the hash are
in the first place, or if they could, you would still be hidden within the range of 300-500 other hashes that start with the same 5 characters, 
which, of course, corresponding to COMPLETELY different passwords.

However, while that site should more than likely be trusted, the best policy with passwords and security will always be: "Trust No one".
That's why instead of entering your password, that is still handled responsibly by the HIBP website, you can use this Python script to read over a text file and
tell you in the terminal whether or not your passwords have been hacked. 
If they have been hacked, it will even tell you just how many times it is known to have been hacked.

This way your password hashes never get sent over the wire, but the list of hundreds of hashes that it COULD be come to you, and then we can 
compare safely on your own device.

I would recommend only doing this on a secure and trusted network of course. Don't try in a coffee shop, folks!
