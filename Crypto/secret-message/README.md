<h1>secret-message</h1>

<h1>Challenge Text</h1>
There are two bank heist organizations communicating by sending images of expensive assets to each other, could there be a secret message somewhere?
Along with the images, they are sending the same secret_key.txt file with encoded text.


<h1>Hint</h1>
The employees of both organizations passed Decoding 101 in high school, but failed Encryption 101 in college.


<h1>Solution</h1>

<ol>
<li>Open the secret_key.txt file - there will be a url encoded string.</li>
<li>Take the url encoded string and decode it - https://www.urldecoder.org/</li>
<li>The decoded url string will output a base64 string, decode it - https://www.base64encode.org/</li>
<li>The decoded base64 string will output a Caesar Cipher encrypted string, decrypt it - https://www.dcode.fr/caesar-cipher</li>
<li>Use the steghide command to unhide the hidden secret_message.txt file. Using the passphrase manchester_united_2022 to unlock the file. Command: steghide extract -sf Photo.jpg</li>
</ol>
 Flag: jctf{QbxVLJrIbP}
