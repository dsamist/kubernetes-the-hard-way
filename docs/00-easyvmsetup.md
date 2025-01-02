To quickly setup a debian VM for this tutorial without installing from an ISO image, I used the one provided by osboxes.org.

Full link [here](https://www.osboxes.org/debian/#debian-12-6-info)

With this, you can just download the vdi file and attache it to your VBOX.

The default username and password is provided in the info tab on the web page.

NB: The machine doesn't come with openssh installed. Hence, remoting to the server initially might not be possible untill openssh is installed. Use command:

sudo apt install openssh-server -y


##### additional notes
Because I am using my local machine as the jump host to the other debians, some changes were made.

1. I created a "downloads" directory in this same pwd (kubernetes-the-hard-way) and here I downloaded the binaries
    * mkdir downloads
    * wget -q --show-progress --https-only --timestamping -P ./downloads/ -i downloads.

2. I have kubectl already installed on my machine, hence, the step was skipped.

3. If you are using an "amd" based system, then ensure that you edit the [download.txt file](../downloads.txt) to reflect the correct binaries. Meaning replace all the "arm" with "amd" in this file. 