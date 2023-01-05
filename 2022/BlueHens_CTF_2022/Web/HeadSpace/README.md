# Headspace
## Web-Exploitation , Curl

##### Description
 - Question : http://bluehens-headspace.chals.io/ (No longer active)
 - Source   : ```No-Long Link```
 - Author   : JR

<ins>Approach:</ins>
- First i think to use the head protocol. But which is not respond.
- So i plan use the curl.
- first of all we got that we have to use flag.org as referer
  ```sh
  curl -H "Referer: flag.org" https://bluehens-headspace.chals.io/
  ```
  - response: Access Denied! You are not using a valid agent. Currently you are using: curl/7.80.0 Valid Agents: stealthmodeactive
- let's change our agent with -A option in curl
  ```sh
  curl -A "stealthmodeactive" -H "Referer: flag.org" https://bluehens-headspace.chals.io/
  ```
  - response: Hmmm you seem to be using the wrong protocol. This server could use a PATCH...
- ok we need to change the method to PATCH. in curl we do it with -X option
  ```sh
  curl -X PATCH -A "stealthmodeactive" -H "Referer: flag.org" https://bluehens-headspace.chals.io/
  ```
  - response: Nice! Hopefully you learned a thing or two about HTTP headers :) UDCTF{0uts1d3_t4h_m1nd}
- Finally flag is gotted.
