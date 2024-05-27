# SSH Bruteforce

## Objective
The goal of the SSH bruteforce project was to simulate how weak passwords containing relations to an employee's organization can be leveraged by adversaries. This project consisted of utilizing a controlled environment along with tools and scripts in Kali linux to extract information from a website (Delta airlines in this example) and using the info to create a wordlist for an SSH bruteforce attack. The purpose was to enhance my understanding of attack techniques, tools, and iterate the importance of strong passwords.


### Skills Learned

- Ability to perform a basic red team engagement.
- Improved proficiency in Kali linux instruments.
- Deployment of SSH server on Windows machine.
- Enhanced awareness of security vulnerabilities.
- Development of problem-solving skills in cybersecurity.

### Tools Used

- Oracle VM
- Kali Linux
- CeWL
- Python Scripts
- Splunk

## Guide

Ref 1: Network Diagram

![Screenshot (1722)](https://github.com/Cyber-ic5/SSH-Bruteforce/assets/169179159/de814200-61d1-42f1-bc89-9ca97e9efd1b)

Ref 2: Using CeWL on Kali to crawl through the 1st 2 pages of the Delta airlines website to scape all words with a minimum length of 6 characters.

![Screenshot (1684)](https://github.com/Cyber-ic5/SSH-Bruteforce/assets/169179159/202aefeb-1891-4554-b0ba-8fea2b252a4e)

Ref 3: The scraped wordlist was piped into a Python script which appends random numbers and symbols.

![Screenshot (1686)](https://github.com/Cyber-ic5/SSH-Bruteforce/assets/169179159/04c5c9c2-5057-4950-b7ca-c3f587f4ba8d)

Ref 4: The newly created wordlist was transferred to a file named "passwords.csv" with the following format.

![Screenshot (1687)](https://github.com/Cyber-ic5/SSH-Bruteforce/assets/169179159/ea506cf5-a155-4dab-bb41-a3d122a453bd)

Ref 5: A python script was launched which uses the "passwords.csv" file to bruteforce an ip.

![Screenshot (1709)](https://github.com/Cyber-ic5/SSH-Bruteforce/assets/169179159/6f46c40b-6a8d-49c6-91f6-d7ecc79fe74f)

Ref 6:
