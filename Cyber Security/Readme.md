# Security Goals (CIA Traid)

![image](https://user-images.githubusercontent.com/35686407/190711247-6f13ea87-7f90-4cb2-8abf-750e02776bc8.png)


1. Confidentiality:
    - 3rd person access na kre
    - sender nae jise send kra hai, use hi send ho
    - bich mae 3rd person access na kre
    - data srf authorized person,institute,organization pd rha hai, then, its confidentiality maintained else it is losed
2. Integrity
    - sender to receiver end,
    - jb tk data pochta nhi, tb tk uska 1 bit bhi idhar se udhar nhi hona chahiye
    - koi bhi modification nhi hona chahiye message ka
    - then it is integrity maintained of data
3. Avaliability
    - jo bhi resources hai, vo authorized bnde ko hmesha avaliable chahiye
    - prime resouce : data
    - then hardware,software,memory
    - maitain rehne chahiye, avaliable rehne chahiye to authorized user

# IS (Information Security)

# Elements of IS

1. Physical Elements:
    - Guard (Like: Manual Checking Guard in Organization)
    - Camera
        - Insann so jata hai, to unauthorized bnde ko cctv camera dekhenge
    - Rzone
        - Restricted Zone Maintained, 
        - insitute mae particular zone mae confidential information secure hoti hai
        - restricted zone
        - authorized access , high level ka bnda
        - normal bnda nhi ja skta
    - Downloading
        - Downloading kuch bhi kr rhe hai altu faltu, uske upar bhi restrictions
    - Access Rights
        - koi ek bnda bndi kaam krti thi, he/she leaves, jitne bhi access rights jude the us bnde se with organization, sare vapis le liye jaye, revoke it cancel it, security issue na ho

2. System Elements:
    - Antivirus
    - Malicious s/w detection solution
    - Disable usb ports

3. Process Elements:
    - Authorized User/ Access Control
    - S/W details
    - log entry

# Security Attacks

1. Passive Attacks
    - A nae B ko data send kia
    - C data ko read krta hai, do not modify that message
    - A and B ko bilkul bhi bhanak nhi lgti ki C unki communication ko observe kr rha hai
    - isliye bhtt mushkil ho jata hai identify krna is attack ko
2. Active Attacks
    - A and B ke bich jb communication kr rha hai
    - C kuch errors daal deta hai us message mae and B ko paas kr deta hai
    - B ke paas curropted message aata hai

# Encryption Techniques (Classical)

1. Substitution Technique
2. Transposition Technique

> Substitution Technique: Letters are replaced by other letters or Symbols

![image](https://user-images.githubusercontent.com/35686407/190844006-c3b50872-1023-454c-a64f-d6a019d887bb.png)

> Transposition Technique: Some sort of permutation on plaintext letters

- If length of text is big, then it is useful.
- ![image](https://user-images.githubusercontent.com/35686407/190844067-b1643117-3de9-41f9-aa0f-4474ff0e94b1.png)


![image](https://user-images.githubusercontent.com/35686407/190844084-bfeb7684-97d2-49bf-8c1b-e7ea4c004f17.png)


# Mono alphabetic Substitutions:

![image](https://user-images.githubusercontent.com/35686407/190844316-6faab851-7587-4a8c-8ff1-679da0cc797f.png)

![image](https://user-images.githubusercontent.com/35686407/190844345-88caa4a9-8101-4b60-b125-c1682f2a7c6f.png)

- If any letter is mapped with some another letter, then it will not mapped to some another letter.
- 26! ways to make the key, if key is found then message will be decrypted. But finding 26! permutations is very huge.

![image](https://user-images.githubusercontent.com/35686407/190844539-d157d1bd-e673-4ec7-a31b-8298f96d312a.png)

![image](https://user-images.githubusercontent.com/35686407/190844476-2aada37a-e7d1-4f4c-ab81-89ca1452cc52.png)

![image](https://user-images.githubusercontent.com/35686407/190844490-4e3c8d7b-eb06-4357-9f48-dee857ee494e.png)

![image](https://user-images.githubusercontent.com/35686407/190844579-0965ce54-a2d2-43e1-a2a2-4b3a2582cbbc.png)

- G has the higher frequency, so it might be E,
- then all letters have same frequency, so we are guessing the letters for each letter in cypher text , with help of relative frequency chart of letters.
- This is Guessing Attack.

![image](https://user-images.githubusercontent.com/35686407/190844688-e116dee7-17e3-4617-9b5b-92c8f27b7a69.png)

- then if  we apply guessing attack then we get,,

![image](https://user-images.githubusercontent.com/35686407/190844714-d0773f17-e639-419f-9a4c-93afbf3a2ea9.png)

- In simple words, Mono-alphabetic cipher mae hum one to one letter mapping krte hia, jisme hum 26 letters ki ek key bnate hai, and english letters ko uske sath map krte hai.
- ![image](https://user-images.githubusercontent.com/35686407/190844785-c6e26fba-fda3-45c6-b0ce-b1750465fd3f.png)
- Example Key: The quick brown fox jumps over the lazy dog, map this with the english alphabets and then encrypt the plain text.

![image](https://user-images.githubusercontent.com/35686407/190844743-b1ae34d6-15a2-4a72-892e-cfd5a840b276.png)

# Polyalphabetic Cipher (Vignere Cipher)

![image](https://user-images.githubusercontent.com/35686407/190845087-23941856-8634-4688-a392-28b837777e19.png)

![image](https://user-images.githubusercontent.com/35686407/190845118-98d28f22-f242-46ba-9227-1d0fe3b58364.png)

![image](https://user-images.githubusercontent.com/35686407/190845183-e080a9b1-6121-4885-ad7a-7c5ab3515b6c.png)

- a: 0, b: 1, c: 2, d: 3 .. and so on 
- PT have eqvalent numbers
- Fill the table and apply formula
- 
![image](https://user-images.githubusercontent.com/35686407/190845221-cb301b68-475d-4ac1-b59a-46ee0af47287.png)

![image](https://user-images.githubusercontent.com/35686407/190845445-4b3ce10d-5438-45ef-b929-ade9d28167a8.png)

![image](https://user-images.githubusercontent.com/35686407/190845522-638b2203-5786-4083-91e5-f6408c31fde2.png)


# Playfair Cipher

- Message : Jazz,
- keyword : Monarchy
- Create 5 x 5 cell
- Insert Row Wise Left to right (Keyword)
- jpo bhi alohabets keyword ke the jo cells mae daal diye hai, unko chord ke, jo 26 standard alphabets hai unme se keyword valo ko hta de, remaining alphabets ko unko cells mae bhrna hai
- Now , kese bhrna hai ?
- 2 alphabet 1 cell mae hoen chahiye tbhi 26 aayenge pure, kyuki 5x5 ka  cell to 25 cell hai.
- j ko hmesha i ke sath likhna hai
![image](https://user-images.githubusercontent.com/35686407/190846846-c54953eb-48e1-413d-8c5d-5d1fa76f44dd.png)
- Table Row Wise bhrna hai
- ab message ko decompose krna hai (todna hai)
- 2 - 2 alphabet pkdne hai
- Repeatition dikh rha hai (e.g. zz) , zx, zx pair bnana hai
- message : jazz (ja, zx, zx)
- jb bhi pair krne ke liye koi alphabet nhi hai, then we append it with x
- jb 2 alphabets repeatiotion mae hote hai, tb usko append krte hai x ke sath
- Example: GREET : (GR, EX, ET)
    - X ko lgane ke liye priority pehle vale E ko deni hai,
- Example: OFF : (OF,FX)

> Working:

- Agar pair ke letters same column mae hai, then unalphabet ke immediate down vale alphabet ko likh denge unke corresponding
- agar pair same row ko belong krte hai, we take right, if alhabet right is not there, we use cyclic order (wrap around)
- Example: OFF (OF, FX)
- Agar same column row mae nhi hai e.g. FX , then create a rectangle, then F and X are diagonal Cells, F and X ke corner opposite points - F ki row mae jo cell content sbse pehle aata hai, use likhna hai , then for F we write i or j anything
- X ka row dekho, uska V aaya, 
- (Clockwise)

![image](https://user-images.githubusercontent.com/35686407/190849235-6d0acf54-7833-4b93-81b4-2f63938e339a.png)

![image](https://user-images.githubusercontent.com/35686407/190849422-0b3ad71b-5b60-4bdf-bd23-cf8c890531fc.png)

![image](https://user-images.githubusercontent.com/35686407/190849444-92676bb7-5944-4ec0-8f99-4bb5334434a2.png)

# Stream Cipher

- jb bhi keys/algo ko every bit of data bit pr apply krte hai, then it is stream cipher
- Example: One Time PAD

![image](https://user-images.githubusercontent.com/35686407/190849765-f7e815fd-0b97-488f-98ca-648796eab763.png)

- Represent Message in terms of bits
- Key Stream generator, generate key in terms of bits (k1 is first key of bit1, and k2 is second key of bit2)
- XOR between them, we got C1,C2,...
- We User Stream Cipher Technique/Algorithm
- ek ek bit ko consider krke key apply kr rhe hai, and cipher text ki bit ko generate kr rhe ho
- then send it to receiver side
- receiver ke paas bhi key stream generator hota hai
- vo uske sath XOR kr deta hai, then we got original message
- EXAMPLE:
    ![image](https://user-images.githubusercontent.com/35686407/190849892-98abd78c-7e6d-4250-80a6-5980d7ad9e01.png)
- There is no error/noise in the message

# Block Cipher

- Plain text ko blocks mae divide kr dete hai of fixed size
- Key apply krte hai each block mae
- Cipher text can also be generated in format of blocks also if plain text is divided into blocks.
- ![image](https://user-images.githubusercontent.com/35686407/190850027-9cb41832-fc70-4ceb-b105-258bbb9dd411.png)
- Key Size: (40,56,64,128,256 Bits) Fixed Size
- vo size ki key, hr ek block mae lgai jayegi
- Example: DES (Data Encryption Standard)
    - Block Size : 64 Bits
    - Cipher Text : 64 bits

# CryptAnalysis

The process of attempting to discover the plaintext or the key or both is known as cryptanalysis.
A cryptanalyst can do any or all these things:
1. Attempt to break a single message
2. Attempt to recognize patterns in encrypted messages,
3. Attempt to deduce the key, in order to break subsequent messages easily
4. Attempt to find weaknesses in the implementation or environment of use of encryption
5. Attempt to find general weaknesses in an encryption algorithm, without
necessarily having intercepted any messages


# Vernam Cipher (One Time PAD)

- Plain text to Cipher text
![image](https://user-images.githubusercontent.com/35686407/191044401-fe280c78-94a3-466c-904c-55b5fb1a9741.png)

- Assign Number to Ea h Alphabet (A : 0, B : 1 ... Z : 25)
- in Hello, pick every alphabet, H ke corresponding key likh do
- Key should be as complex as possible
    - Rule: Plain text ki length hai, utni hi length ki key leni hai
    - Key can be random.
- Write key ke numbers also
- Now, add both numbers respectively.
- Then, Subtract , it means, observe these numbers, agar koi bhi addition , isme se > 26 hai, then us particular number ko hi 26 mae se subtract krna hai (x - 26).
    - 34 > 26 , 34 - 26 = 8
    - 35 > 26 , 35 - 26 = 9
- Then write corresponding alphabets from numbers.
- **Hr ek message ke liye new key generate krni pdegi**


# Transpositions Cipher
- Positions change kro alphabets ki,

## Columnar Transpositions Cipher

- Column ko importance mil rha hai
![image](https://user-images.githubusercontent.com/35686407/191049776-fb2caa41-1083-4095-8c20-e51c8e28fe17.png)

- Cols 5 lene hai.
- Row wise insert kro
- key ka column uthao, and write kro

## Keyless Transposition Technique

- write in zigzag manner
![image](https://user-images.githubusercontent.com/35686407/191050835-bda3e7fd-953f-4891-97f3-c76e16729a60.png)
- Write Cipher text row wise left to right

# CryptoSystem

- implementation of cryptographic techniques
- to provide information security services.
- cryptosystem is also referred to as a cipher system.
![](https://www.tutorialspoint.com/cryptography/images/cryptosystem.jpg)

## Components of a Cryptosystem
- Plaintext
- Encryption Algorithm.
- Ciphertext
- Decryption Algorithm
- Encryption Key.
- Decryption Key.

## Types of Cryptosystems
- Symmetric Key Encryption
    - same keys are used for encrypting and decrypting
- Asymmetric Key Encryption
    - different keys are used for encrypting and decrypting the information

# Symmetric Key CryptoGraphy

- only 1 key is used, that key is called symmetric key
- only that key is used in sender end and reciever end, therefore it is known as symmetric key cryptography
- That key is known as secret key
- Encryption process sender end pr ki jati hai
- Decryption process receiver end pr preform ki jati hai
![image](https://user-images.githubusercontent.com/35686407/191052088-a4ce60f7-8897-401b-a177-62d5f6b705ea.png)


![](https://www.tutorialspoint.com/cryptography/images/symmetric_key_encryption.jpg)

- Sender send krna chahta hai message receiver ko
- So, tranmission mae attacker honge, jo message ko read kr lenge, then we use encryption algorithm
- Output is encrypte message
- Now, it sended to the receiver side,
- and decryption is done in reciver side
- Advantage: Complexity of implementation is less
- Disadvantage: if attacker steal the key, and applied to the message, then the message will be read by attacker

## Asymmetric Key

-  Sender and Receiver ke paas public key honi chahiye,
-  Online Repositery mae public key ho skti hai,
-  Private key: Jisko share nhi kiya gya hai use private key kehte hai,
-  dono ends ko private key ke bare mae kuch bhi nhi pta hai.
-  Ab A nae Send krna hai B ko message, then A, B ke public key ko use krke send krega message B ko, then B use apni private key se decrypt krega and read krega message.

![image](https://user-images.githubusercontent.com/35686407/191064328-0379e206-9e7f-44f5-b80b-383d4c965221.png)

![](https://www.tutorialspoint.com/cryptography/images/asymmetric_key_encryption.jpg)

# Deffie Hellman Algorithm of Key Exchange

- Used in Symmetric key Cryptosystem
    - Private key Encryption

- Deffie Hellman, make the formula to exchange the keys
- Take 2 numbers p and q
- p is premitive and q is prime number
- p^x mod q
- e.g. p = 3 and q = 7
- ![image](https://user-images.githubusercontent.com/35686407/191068469-746006f5-eb25-4f00-89fe-9f9ea7a3fae2.png)
- values after mod shoud be different, should not be same
- jiski value repeat na ho mod lene pr, vo primitive root hota hai, p ko esa choose kro ki uski powers ka mod agar lenge q se to vo repeat numbers produce nhi krega
- Alice ke paas key 'a'
- Bob ke paas key 'b'
- A = p^a mod q
- B = p^b mod q
- A send msg to B
- B send msg to A
- Now Alice have message B, and Bob has message A
- now alice and Bob find the private key
- S = B^a mod q
- S = A^b mod q
- Now, S values are same, private key is exchanged bina kisi ko pta chle

- Example:
- q = 13, p = 6
- Alice a = 3
- Bob b = 10
- A = 6^3 mod 13 = 8
- B = 6^10 mod 13 = 4
- now they excahnge 8 and 4
- A = 4 and B = 8
- S = B^a mod 13 = 8^3 mod 13 = 12
- S = A^b mod 13 = 4^3 mod 13 = 12
- Now, private key is 12,12
- and publick= key are A = 8 and B = 4

# Public Key Cryptography (Asymmetric key CryptoGraphy)

![image](https://user-images.githubusercontent.com/35686407/191072521-575d8d4e-0d77-4167-8e07-9411a53fc29f.png)


# Elgamal Algo (Asymmetric Key Cryptography)

![image](https://user-images.githubusercontent.com/35686407/191072084-a2df7929-ebbf-4bf7-98bb-60503d3e214f.png)











































