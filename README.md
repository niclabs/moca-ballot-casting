# CastBallot
Fifth part of the project [*Voter-Ballot Self Verification*](www.cjgomez.cl).

Record and uploads the encrypted ballot of the selection of the voter to the Bulletin Board server, subsequently to verify the signature.

## Files
1. **CaptureQRBallot_Reader_CORE.java**:
2. **CaptureQRBallot_Reader_light.java**:
3. **CaptureQRBallot_Reader_swing.java**:
4. **CaptureQRBallot_Camera.java**:
5. **VoterPublicKey.java**:

## How to Use
* Download the .jar file [here](http://www.cjgomez.cl).
* Put the file castBallot.jar in the project folder.

### Configuration
* Execute ballotVerification.jar with `$ java -jar castBallot.jar`
* Select "Configure Public Information" (just the first time) to setup the address of the Bulletin Board server where will be downloaded the public information of the voter to verify the signature, and uploaded the encrypted ballot.

### Casting Process
* After configuration, select "Initialize Casting".
* Next, the program asks for the voter id who is casting the ballot.
* Then, the program asks to read the encrypted QR-Code value.
* The program downloads the public information of the voter and verifies the signature. 
* If success, the program uploads the encrypted ballot to the Bulletin Board server.
* After this, the program finishes, waiting for the next voter to cast her ballot.