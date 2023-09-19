# Electrum-Wallet-Termux
How to create an Electrum financial wallet using Termux.💵💵


. Here is a step-by-step guide:

1. Update and upgrade Termux:
   ```
   pkg update && pkg upgrade
   ```

2. Install needed packages:
   ```
   pkg install python
   pkg install git
   pkg install wget
   ```

3. Clone the wallet software repository:
   ```
   git clone <wallet-software-git-repo-url>
   ```

   Replace `<wallet-software-git-repo-url>` with the URL of the wallet software's Git repository. For example:
   
   - Electrum: https://github.com/spesmilo/electrum.git

👇👇
```git clone https://github.com/spesmilo/electrum.git```

4. Go to the wallet software directory:
   ```
   cd <wallet-software-directory>
   ```

   Replace `<wallet-software-directory>` with the directory where the wallet software was cloned. For example:
   - Electrum: `cd electrum`

👇👇
```cd electrum```
👆👆

5. Install the wallet software's dependencies:
   ```
   pip install -r contrib/requirements/requirements.txt
   ```

6. Configure and create a wallet:

   - Electrum:
     ```
     python3 -m venv .env
     source .env/bin/activate
     python -m pip install --upgrade pip
     pip install <wallet-version>
     ```

     Replace `<wallet-version>` with the specific version you want to install (e.g., `electrum==4.4.6`).


👇👇
     ```python3 -m venv .env 
  source .env/bin/activ ate   
     python -m pip install --upgrade pip
     pip install <4.4.6>
     ```
👆👆

     `To create a new Electrum wallet:`
     
```electrum create```
    

  
     `Follow the instructions on the screen to set up your wallet and passphrase.`

7. Generate wallet addresses:

   - Electrum:
     ```
     electrum getunusedaddress
     ```

8. Secure your wallet:
   - Enable two-factor authentication if supported by the wallet software.
   - Regularly back up your wallet using the wallet software's recommended method.
   - Don't share sensitive wallet information like your passphrase.

9. Make payments and receive payments:

   - Electrum:
     ```
     electrum payto <receiver-address> <amount>
     ```

     Replace `<receiver-address>` with the address of the recipient and `<amount>` with the amount to send.

Remember to refer to the official documentation or relevant resources provided by the specific wallet software you choose for accurate and detailed instructions.