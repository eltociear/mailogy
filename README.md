# Mailogy

https://github.com/granawkins/mailogy/assets/50287275/202f28fc-d148-4666-a6d0-dd02fc2a0b63

Interact with your email records using natural language. You can say:

* “Give me every receipt in my inbox in CSV format, with the following columns: gmail link to the email, sender email, sender name, amount in the receipt.”
* “Give me every subscription in my inbox including cancelled subscriptions. ""
* “Tell me every service I’ve ever logged into or signed up for along with time of last login”

## How to Download Your Gmail as a .mbox File

To download your Gmail emails in `.mbox` format, follow these steps:

1. Go to your Google Account by navigating to https://myaccount.google.com/.
2. On the left navigation panel, click on `Data & privacy`.
3. Scroll down to the `Data from apps and services you use` section and click on `Download your data`.
4. You will be redirected to the Google Takeout page. By default, all data types are selected. Click on `Deselect all`.
5. Scroll down to `Mail` and check the box next to it.
6. You can choose to include all your email labels or select specific labels by clicking on `All mail data included`.
7. After making your selection, scroll down to the bottom of the list and click on `Next step`.
8. Choose your preferred file type, frequency, and destination for the data export. For `.mbox` files, you can leave the default settings.
9. Click on `Create export`. Google will then prepare your download, which may take some time depending on the amount of data.
10. Once the export is ready, Google will email you a link to download your `.mbox` file. Follow the instructions in the email to download the file to your computer.

## Usage Guide

> **Note:** You will need an OpenAI API key to run this program. You can set it as an environmental variable, otherwise your will be prompted to enter your first time.

1. Clone this repo using the following command:

    ```
    git clone http://github.com/granawkins/mailogy
    ```

2. Install the required dependencies with pip:

    ```
    pip install -r requirements.txt
    ```

3. To process your `.mbox` file, run the program using the following command:

   ```
   python -m mailogy path_to_your_mbox_file.mbox
   ```

   Replace `path_to_your_mbox_file.mbox` with the actual path to your `.mbox` file.

4. Follow the on-screen prompts to interact with the program and process your email records using natural language commands.

5. After your `.mbox` file has been processed, can load your complete library again (without delay) by running:

    ```
    python -m mailogy
    ```

    If you do include a path, you will be guided through the same procedure as #3. 
