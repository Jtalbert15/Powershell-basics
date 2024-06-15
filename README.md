# Powershell-basics
<img width="279" alt="Screenshot 2024-06-15 at 4 36 40 PM" src="https://github.com/Jtalbert15/Powershell-basics/assets/66844406/e83ccfe3-5f3e-440c-830f-4f8254de269e">

<h1>Summary</h1>
In this lab we'll go over some Powershell basics. We will go over how to change which directory we are in, creating a directory, using the ipconfig command, and using the pipeline to chain commands.

<h1>Changing Directories with cd</h1>

To start, open up Powershell

<img width="836" alt="Screenshot 2024-05-31 at 8 06 20 PM" src="https://github.com/Jtalbert15/Powershell-basics/assets/66844406/d5c669e0-1568-4e10-b414-60ea1b2f8f73">

We can navigate our file structure using cd. Cd stands for change directory.

We can see we are currently in the C drive in the administration folder which happens to be inside the users folder

To go back in our file structure we can type cd ..\ and hit enter

<img width="853" alt="Screenshot 2024-05-31 at 8 12 01 PM" src="https://github.com/Jtalbert15/Powershell-basics/assets/66844406/c2ce74e7-6658-4e8b-aa28-44e1702d53f3">

Now we can see that we are in the users folder within the C drive

<h1>Step 2) Creating a Folder with the mkdir command</h1>
Let's create a folder to do that we can type mkdir

mkdir (make directory) will create a folder where we are located in our file structure

we need to create a name for this folder so we can type mkdir followed by the name of your folder 

<img width="414" alt="Screenshot 2024-05-31 at 8 23 49 PM" src="https://github.com/Jtalbert15/Powershell-basics/assets/66844406/e0554852-8bcc-471e-9e8d-07ae0c653a20">

Now we can navigate to that folder by typing .\new_folder

Powershell has a cool feature where it will autocomplete

You can use this by typing partially of what folder you want to access and pressing tab

If the result is not what you wanted you can press tab until you select the right file

<img width="249" alt="Screenshot 2024-05-31 at 8 29 30 PM" src="https://github.com/Jtalbert15/Powershell-basics/assets/66844406/fa0bfeee-506f-4b90-b36f-321a7ab710c4">

Now we are in our new folder
<h1>Step 3) Checking Network Information with ipconfig</h1>

Now lets take a look at our network configuration

Type ipconfig /all

Then press enter

<img width="836" alt="Screenshot 2024-05-31 at 8 44 54 PM" src="https://github.com/Jtalbert15/Powershell-basics/assets/66844406/e11cb5b8-fd0f-446d-a00d-ba601b00810b">

Now we can see a bunch of information about our network

Now lets clear our terminal type clear and then hit enter

<img width="835" alt="Screenshot 2024-05-31 at 8 46 24 PM" src="https://github.com/Jtalbert15/Powershell-basics/assets/66844406/39b0ce81-1c40-4f1d-b316-27bfd1e4076c">

That was a lot of information in our terminal we can filter down our information

<h1>Chaining Commands with the Pipeline</h1>
<img width="433" alt="Screenshot 2024-05-31 at 9 00 06 PM" src="https://github.com/Jtalbert15/Powershell-basics/assets/66844406/6e2949b6-6957-4a05-b3a1-e625b7afb7ae">

Breaking down the code up above we see the code we inputed earlier

To the right of that code you can see a |

This allows us to take the output of the code to the left of the symbol

And input it into the right side of the symbol

in this case select-string grabs the string that contains the term ipv4 in it

<img width="456" alt="Screenshot 2024-05-31 at 9 03 53 PM" src="https://github.com/Jtalbert15/Powershell-basics/assets/66844406/facc1661-9feb-4036-b82e-acc72f2a53e2">



