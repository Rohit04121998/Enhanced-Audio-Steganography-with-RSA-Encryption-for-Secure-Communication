# Enhanced-Audio-Steganography-with-RSA-Encryption-for-Secure-Communication

Audio steganography is an efficient method to secure embedded data and sent it through internet. Unfortunately, the integrity of the message may be compromised with only the use of LSB method to hide data.  Hence, To provide secure communication by integrating Steganography on Audio Files along with an Encryption Algorithm such as RSA is proposed.

## Need for audio steganography

Rapid and sudden increase in the Transmission of digital data over the Internet forced researchers for enhancement in the security system. Steganography is the art of 'secret
writing'. It conceals the existence of a hidden message and allows it to be only extracted by intended recipient. Embedding secret data in digital audio cover is more challenging than using digital images as a cover since human visual system is less sensitive in comparison to human auditory system. Audio Steganography includes concealing information
in audio records. This technique conceals the information in WAV, AU and MP3 sound records. The advantage of steganography, over cryptography alone, is that messages do not attract attention to themselves. They have the potential capability of hiding the existence of confidential data thus eliminating any need for suspicion.

## Method

The proposed work aims to leverage the added benefits of steganography and en- cryption mechanisms to counter any drawbacks presented by these individual techniques. Implementation of data hiding using the LSB technique is presented in conjunction with the RSA encryption standard. A Graphical User Interface is also built to make the entire process user friendly and smooth.

The proposed algorithm was developed using Python and a GUI was built using the *tkinter* library provided by Python. Encoder and decoder modules were built. RSA was implemented along with the generation of prime numbers and secret keys. Lastly, the hiding and extraction of the text message in the audio file was shown with no change in the size of the file.

<p align="center"><img src="https://github.com/Rohit04121998/Enhanced-Audio-Steganography-with-RSA-Encryption-for-Secure-Communication/blob/main/Design%20Methodology.png" height="400"></p>

## RSA Encryption

Rivest-Shamir-Adleman," or RSA, is another prominent encryption method. It is frequently used to encrypt data transferred over the internet and depends on a public key to do so.

<p align="center"><img src="https://sectigostore.com/blog/wp-content/uploads/2020/06/how-rsa-works.png" height="400"></p>

### <p align="center">Working of RSA Encrpytion</p>

The RSA algorithm is a type of asymmetric cryptography algorithm. Asymmetric indicates that it operates on two distinct keys, namely the Public Key and the Private Key. The Public Key is distributed to everyone, whereas the Secret Key is kept private, as the name implies. Those receiving the data will be given their own private key to decode the communications. It has been shown to be a secure method of sending information between persons who may not know each other yet wish to connect without exposing their personal or sensitive data.

RSA has various advantages which include, but are not limited to:

* RSA algorithm is safe and secure for its users through the use of complex mathematics
* It is hard to crack since it involves factorization of prime numbers which are difficult to factorize
* It uses the public key to encrypt data and the key is known to everyone, therefore, it is easy to share the public key

## Implementation

* The audio file worked on has a .wav format. One of the reasons .wav audio format is used is it provides lossless compression format
* LSB and RSA programs are integrated.  The sender prompts the receiver that it wants to send a message
* The receiver makes two sets of keys (One private and One public) and shares the public key to the sender but keeps the private key to itself.  The sender encrypts the data with the key and puts it on the audio wav file
* Encoder  module  calculates  all  the  frame  bytes  of  the  audio  file  and  changes  the last bit of each byte to store the encrypted data.  On the receiver side the decoder module decodes the encrypted data from the audio.  It then calls the receiver module
* The data is then decrypted by the receiver module using its private key

<p align="center"><img src="https://github.com/Rohit04121998/Enhanced-Audio-Steganography-with-RSA-Encryption-for-Secure-Communication/blob/main/GUI.png" height="400"></p>

### <p align="center">GUI</p>

## Future Scope

While steganography is an excellent technique for data hiding, the duration of the message is limited by the song. Therefore, there is a need to discover new methods so that more information can be transmitted through the same song. Moreover, the whole system can be available on the Cloud, giving users a better experience.
