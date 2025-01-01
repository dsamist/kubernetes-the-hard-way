To quickly setup a debian VM for this tutorial without installing from an ISO image, I used the one provided by osboxes.org.

Full link [here](https://www.osboxes.org/debian/#debian-12-6-info)

With this, you can just download the vdi file and attache it to your VBOX.

The default username and password is provided in the info tab on the web page.

NB: The machine doesn't come with openssh installed. Hence, remoting to the server initially might not be possible untill openssh is installed. Use command:

sudo apt install openssh-server -y