# Story-Protocol

Download Genesis & Addrbook

    curl -o genesis.json https://raw.githubusercontent.com/Validator247/Story-Protocol/main/genesis.json
    curl -o addrbook.json https://raw.githubusercontent.com/Validator247/Story-Protocol/main/addrbook.json 

Upgrade

        cd $HOME
        rm -rf story
        git clone https://github.com/piplabs/story
        cd $HOME/story
        git checkout v0.10.0
        go build -o story ./client
        sudo mv $HOME/story/story $(which story)
        sudo systemctl restart story && sudo journalctl -u story -f

                
