---
layout: default
---

**Legal / Ethical Notice:**  
This site is for educational purposes only. Do **not** use the materials here for illegal activity. All code samples are non-actionable and designed for learning in isolated environments.

***

**What is Malware Obfuscation?**


***

**Three Common Methods of Obfuscation**

*Software Packing*

*Encrypted/encoded Files or Strings*

*Command/Script Obfuscation*


***

**Steganography**

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
