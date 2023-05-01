Download Link: https://assignmentchef.com/product/solved-blockchain-homework-1
<br>
<ol>

 <li>Find a collision in each of the hash functions below:

  <ol>

   <li>H(x) = x mod 7<sup>12</sup>, where x can be any integer</li>

   <li>H(x) = number of 1-bits in x, where x can be any bit string</li>

   <li>H(x) = the three least significant bits of x, where x can be any bit string</li>

  </ol></li>

 <li>Prove the statement: In a class of 500 students, there must be two students with the same birthday.</li>

 <li>Find an x such that H (x ◦ id) Y where

  <ol>

   <li>H = SHA-256</li>

   <li>id = 0xED00AF5F774E4135E7746419FEB65DE8AE17D6950C95CEC3891070FBB5B03C77</li>

   <li>Y is the set of all 256 bit values that have some byte with the value 0x1D.</li>

  </ol></li>

</ol>

Assume SHA-256 is puzzle-friendly. Your answer for x must be in hexadecimal. You may provide your code for partial credit, if your x value is incorrect. You may use the accompanying CryptoReference1.java file to help you with this question. Submit both your code and your value of x.

Notes:

<ul>

 <li>The notation “x ◦ id” means the byte array x concatenated with the byte array id. For example, 11110000 ◦ 10101010 is the byte array 1111000010101010.</li>

 <li>The following two code segments are <strong>not</strong> equivalent:</li>

</ul>




<table width="602">

 <tbody>

  <tr>

   <td width="289"><strong>Segment 1 </strong><strong> </strong>String val = “0x1D253A2F”; if (val.contains(“1D”))    return true;</td>

   <td width="313"><strong>Segment 2</strong>byte[] val = new byte[]{0x1D,0x25,0x3A,0x2F} for (byte b : val)    if (b == 0x1D) return true;</td>

  </tr>

  <tr>

   <td colspan="2" width="602">The second code segment above is the correct way to check whether 0x1D is a byte in 0x1D253A2F.</td>

  </tr>

 </tbody>

</table>

Remember that hex format is only a way to represent a byte sequence in a human readable format. You should not be performing operations directly on hex-string representations. Instead, you should first convert hex-strings into byte arrays, then perform operations on the byte arrays directly, and then convert the final byte array into a hex format when giving your answer. Performing operations directly on the hex strings is incorrect.




<ol start="4">

 <li>Alice and Bob want to play a game over SMS text where Alice chooses a number between 1 and 10 in her head, and then Bob tries to guess that number. If Bob guesses correctly, he wins. Otherwise, Alice wins. However, Bob complains that the game isn’t fair, because even if Bob guessed correctly, Alice could lie and claim that she chose a different number than what she initially chose. What can Alice do to prove that she didn’t change the number she initially chose? Devise a mechanism to address Bob’s concern. Provide a detailed explanation of the mechanism and why it works. An answer with insufficient detail will not receive credit.</li>

</ol>