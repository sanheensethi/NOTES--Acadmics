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



















































