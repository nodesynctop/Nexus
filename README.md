# How to run Nexus Testnet CLI command


## Step 1: Install required packages
```
sudo apt update && sudo apt upgrade -y
sudo apt install build-essential pkg-config libssl-dev git-all protobuf-compiler -y
```
```
curl --proto '=https' --tlsv1.3 https://sh.rustup.rs -sSf | sh
. "$HOME/.cargo/env"
```
## Step 2: Get PROVER ID: https://beta.nexus.xyz (bottom left) and run the command below, enter your prover id
```
curl https://cli.nexus.xyz | sh
```
## Step 3: Run the above command, Ctrl + c (stop and manually enter the command below, because I see the prover id is not added by the auto command above)
```
echo "YOUR_PROVER_ID" > ~/.nexus/prover-id
```
Example: `echo "abcxyzzzzzzzzzzzzzz" > ~/.nexus/prover-id`

## Step 4: Run the command again to restart (remember to hang the command in tmux or screen to monitor logs)
```
curl https://cli.nexus.xyz | sh
```
## Step 5: Go back to https://beta.nexus.xyz, Go to My profile to see if the CLI node shows up, wait about 5 minutes

![nuxus](https://github.com/user-attachments/assets/0dc80382-d95b-42fe-af29-2a214cb92ad2)
`Note:` Go to My Profile, fill in your email, save, and confirm email
