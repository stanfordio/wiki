# Tails Installation Instructions
## Why Tails?
These days, you can't really trust anything you find on the internet, but the risk is especially high if you're researching shady actors that operate in the darkest corner of the web. Generally, any link you visit outisde of a trusted site (like Google or Facebook), as well as any attachment you download and open, could expose you to some nasty risks. There are a few actions you can take in the course of your daily research to mitigate these risks. A main one is using Tails as a virtual machine to do risky things on the internet.

[Tails](https://tails.boum.org/) is an operating system designed to keep you anonymous on the internet by default. It's a flavor of the Linux line of operating systems that uses [Tor](https://www.torproject.org/) by default. Tor is a effectively a special kind of VPN that anonimizes your traffic by ping-ponging it around the world before sending it to its destination. In any given session, you might be sending from Norway, Columbia, Thailand, or Algeria, making you difficult to track.

Additionally, by containing risky internet browsing to a virtual machine (VM), even if someone successfully compromises your machine, you can just flush your VM image and start anew, infection-free. You'll be free to click as many sketchy Russian links as your heart desires (within reason of course).

Note that this will not protect you against every threat (nothing ever does). For example, if the VM is compromised and you pull files from your VM to your actual MacOS file system, you may expose your actual computer to an infection. Also, if your attacker is smart enough to worm through the local network once infecting your VM, there isn't very much you can do there. As with everything internet security related, just be vigilant and overly-cautious and you should generally be OK.

## Installation Guide
Below are instructions for getting a Tails VM up and running.
1. ## Download and install VirtualBox
VirtualBox is a program that runs virtual machines from your local computer. If you're curious how this works, [here](https://www.makeuseof.com/tag/virtual-machine-makeuseof-explains/)'s a decent explanation at the layperson level. You can find install instructions [here](https://www.virtualbox.org/wiki/Downloads). Note: on MacOS, you might run into a security error with the package installer. Follow the prompts to create a security exception in Settings, aftwards it should work if you retry the install from the downloaded `.pkg`.
2. ## Download Tails ISO
An [ISO](https://en.wikipedia.org/wiki/ISO_image) is a disk image -- what's burned onto CDs and DVDs. It's also how operating system images are generallyl stored. Download the Tails ISO from [here](https://tails.boum.org/install/vm-download/index.en.html), making sure to select `Direct Download` and to note to where you've downloaded it.
3. ## Install Tails VM
Follow these instructions on how to create a Tails VM Image from your downloaded ISO. Note: At step 4, if you want the VM to have persistent storage (i.e. not have the hard drive wiped every time you shut down the image), you'll want to deviate from the instruction here and choose `create new virtual disk`. Click through the default suggestions from there and you should be able to continue with the instructions without incident.
4. ## Run It
Click on the new VM and select `Run`. If you're on MacOS, you're going to get a lot of permissions requests that are automatically blocked (like for keyboard access). Click through everything to approve any permissions VirtualBox asks for. You might have to Quit (close) VirtualBox a few times for the changes to take effect. Once everything works, start up the VM again and click through the setup prompts. Congrats, you're now using Tails! Go to applications -> internet -> TOR browser to start using the internet.

# Using Tails
You should be using Tails for the following things:
1. Clicking links to sites you've never heard of
2. Opening PDFs from sketchy people (or people in contact with sketchy people)
3. Browsing sites that might have foreign actors looking to track you

Happy sleuthing!