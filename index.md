---
layout: default
---

<ins>**Legal / Ethical Notice:**</ins>  

This site is for educational purposes only. Do **not** use the materials here for illegal activity. All code samples are non-actionable and designed for learning in isolated environments.

***

<ins>**What is Malware Obfuscation? ([T1027](https://attack.mitre.org/techniques/T1027/))**</ins>

For adversaries to introduce their malware into a target system, they must attempt to bypass detection systems that are becoming more commonplace and sophisticated. Obfuscation is the act of making their payload appear differently in order bypass these systems, whether in the files entirety or sections that would be more easily discovered. There is a number of ways that adversaries can carry this out, and more are being developed constantly, a database is maintained by [MITRE ATT&CK](https://attack.mitre.org/techniques/T1027/) and these obfuscation methods are just some of the ways that defense systems are evaded.  


***

<ins>**Three Common Methods of Obfuscation**</ins>

**Software Packing ([T1027.002](https://attack.mitre.org/techniques/T1027/002/))**

After making a new malware program, adversaries will consider having it enter a system without being recognised by antivirus signatures. Software packing is performed by making the program, or components of it, smaller through compression using pre-existing or custom packing programs such as [UPX](https://upx.github.io/). Once in a system, payloads are commonly unpacked in memory and are not detected until the executable is running.

The [Emotet malware](https://www.fortinet.com/blog/threat-research/deep-dive-into-emotet-malware) utilises software packing as part of it's attack, delivered through a malicious word document payload. Once the macro is executed, it downloads a custom packed payload and begins the malware infection to leave a persistent payload.

**Command/Script Obfuscation ([T1027.010](https://attack.mitre.org/techniques/T1027/010/))**



**Encrypted/encoded Files or Strings ([T1027.013](https://attack.mitre.org/techniques/T1027/013/))**



***

<ins>**Steganography ([T1027.003](https://attack.mitre.org/techniques/T1027/003/))**</ins>

Steganography is the concealment of information within a different representation, a historic example is the shaving of a greek servant's head to tattoo a message on their scalp and hide it under their regrown hair. In the digital context, this can be seen with malicious contents being hidden in files such as pictures, documents, or program macros (as seen in the methods above), that to the human eye or surface-level analysis appear benign.

<figure>
  <img src="./images/c62588eb7353-article-200206-steganography-example.png" alt="Steganography hides data in plain sight, image missing" height="200px" width="400px">
  <figcaption>Steganography hides data in plain sight (Dickson, 2020)</figcaption>
</figure>
<br/><br/>
The linked demonstration is a **client-side** script that will take a PNG format image and hide, or extract, a text string utilising the least significant bits (LSB) method, specifically the blue channel (of the RGB data). If you wish to validate that it actually alters the image, feel free to hash the output image files.

[Steganography demo](https://gutbug.github.io/SecPrin-obfuscation-research-project/demo/stego.html)

***

**Key Takeaways and Further Reading**
