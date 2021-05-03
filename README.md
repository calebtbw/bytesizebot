# Bytesize Bot
Currently, this auto-checkout bot will support Best Buy. 

* Easy to use interface built on PyQt5
* Waits for items to restock if they are out of stock
* Optional price checker
* Lighting fast auto-checkout

## Current Functionality

| **Website** | **Auto Checkout** | **Open Cart Link** | **Work In Progress** |
|:---:|:---:|:---:|:---:|
| bestbuy.com |`✔`|`✔`| |

## Bytesize Bot Repository Link
[View The Repo Here](https://github.com/calebtbw/Bytesize-Bot)

## Quick Install for Windows
1. Make sure your Chrome browser is updated to the latest
2. Open Powershell as Administrator within your desired directory for the application to live.
3. Run the following commands: 
      ```
      git clone https://github.com/calebtbw/Bytesize-Bot
      ```
      ```
      cd Bytesize-Bot
      ```
      ```
      python -m venv ./env
      ```
      ```
      ./env/Scripts/activate
      ```
      ```
      python -m pip install --upgrade pip 
      ```
      ```
      pip install -r requirements.txt
      ```
4. If you encounter any errors during installation, please consider the following:
    * If you get a red text error remove and you previously installed pyqt5 or lxml on your python, remove the versions from the **requirements.in** for both lxml and pyqt5, then run the following commands:
    ```
    pip install pip-tools==5.5.0
    ```
    ```
    pip-compile --generate-hashes --no-index --output-file=requirements.txt requirements.in
    ```
    ```
    pip install -r requirements.txt
    ```
    * If you get an error with red text run the following: 
     ```
     pip install pycryptodomex
     ```
5. Run the following command:
   ```
   python app.py
   ```

## Windows FAQs
To resume working on the bot for testing after closing powershell, navigate again to the folder and run the following commands:
  ```
  ./env/Scripts/activate
  python app.py
  ```