# How to configure staticSearch

## Starting off

For starters I have OneDrive disabled but for some reason it still shows up as a file directory when I am file hopping. So, I have to type OneDrive in as a file directory before I start anything in a command line.

Then I get to the correct file directory for Digit 400 and begin starting to configure staticSearch.

## Downloading Steps



1. I began by going to get the staticSearch documents from GitHub and cloning it into my chosen file directory. This link will take you to staticSearch on GitHub so that you can clone it: [staticSearch on GitHub](https://endings.uvic.ca/staticSearch/docs/howDoIGetIt.html)
1. Then, I had to download and install Java to my computer because I did not previously have it. So I clicked this link to download it to my windows: [How to Download Java](https://www.makeuseof.com/windows-11-install-java-jdk/). 
1. Next, I downloaded and installed the latest version of Apache Ant from this link: [Download Apache Ant](https://ant.apache.org/). Then, I unzip the the "ant" folder that contains the `/bin` directory.
1. Afterwards, I download and install the latest version of Ant Contrib into the `lib/` directory of the "ant" folder. I downloaded Ant Contrib by using this link: [Click to download Ant Contrib](https://ant-contrib.sourceforge.net/). This is the latest version of Ant Contrib: [Latest version of Ant Contrib](https://sourceforge.net/projects/ant-contrib/files/ant-contrib/1.0b3/)
1. when you have Ant Contrib downloaded go into the files until you find one with the extension `.jar`. Copy that into the `lib/` folder of "ant" so that ant can use it properly.

## Continuing the Steps to Configuring staticSearch

1. Set ANT_HOME and JAVA_HOME with this link: [Setting up](https://ant.apache.org/manual/install.html)
1. Create a local web server with Python using this link: [Making a local web server with Python](https://ryanblunden.com/create-a-http-server-with-one-command-thanks-to-python-29fcfdcd240e).
1. Install WSL on Windows using this link: [Download and install WSL](https://learn.microsoft.com/en-us/windows/wsl/install). Make sure it's the default Ubuntu shell.
1. Restart you machine to fire up Ubuntu, and then open Ubuntu.
1. Follow the prompt to give youreself a username and password. Make sure you write down your username and password, you will need to remember it for later.
1. Enter this in the Ubuntu terminal to edit in your environment: `sudo nano /etc/environment`.
1. Set up your JAVA_HOME with this code: `JAVA_HOME="/usr/lib/jvm/java-ENTER_WHATEVER_YOU_HAVE_HERE"`.
1. Set up your ANT_HOME with this code: `ANT_HOME="/mnt/c/Users/ebbon/ant/apache-ant-1.10.12"`.
1. You may create easy access alias' to get to your file directories faster as well. For example type: `alias GitHub="cd /mnt/c/Users/*username-you-created*/Documents/GitHub"`
1. Refresh Ubuntu so it recognizes the changes made with this code in the terminal: `source /etc/environment`.
1. Navigate to your staticSearch and run ant.
1. Run your staticSearch in the `/test` directory. 
1. If it works, run `python -m http.server 8000`. OR in my case `python 3 -m http.server 8000` because I have Python 3.
1. Open Google Chrome or Firefox and type in the URL: `localhost:8000` to see if your website went through.




