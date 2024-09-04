### Phaser Game Dev: Galactic Showdown 

PLEASE READ:

    Game was first developed as a client-side only game (client_side_version), and then was converted
    as a multiplayer game with the implementation of the authoritative server architecture which
    involved significant amount of socket programming and its subsequent deployment onto GCP.
    We have provided both versions so that local testing of the functionality can be done since
    the GCP server will only be live for a certain period of time leaving the Multiplayer Folder
    as essentially useless unless grader decides to use their own GCP account for testing. The 
    official project is the following folder: (multiplayer_version):







Client-Side Folder:
    go to correct path:

    REPO
    |--README.md
    |---multiplayer_version
    |---client_side_version/
        |---src/  *** run commands in this directory ***
            |---static
            |---templates
            |---workflow
            |---Dockerfile
            |---requirements.txt
            |---app.py 

    install dependencies: pip3 install -r requirements.txt
    run: python3 app.py



Multiplayer Folder:
    go to correct path:

        REPO
        |--README.md
        |---multiplayer_version
        |---client_side_version/
            |---src/  *** run commands in this directory ***
                |---static
                |---templates
                |---workflow
                |---Dockerfile
                |---requirements.txt
                |---app.py 

    install dependencies: pip3 install -r requirements.txt
    run (locally): python3 app.py
    run (remotely): 

        # Step 1-4 done for user, skip to 5:

        1. containerize on Docker
        2. deploy container to GCP
        3. create firewall rule
        4. create VM instance
        5. run url -> 34.136.116.182:5555

### To play:
    1. click both "Player 1 Ready" and "Player 2 Ready"
    2. Player 1 Controls: { Movement: WASD | Laser: L }
    3. Player 2 Controls: { Movement: Arrows | Laser: SPACEBAR }
