# Pi-Hole Android Private DNS Installer

<img src="https://raw.githubusercontent.com/varunsridharan/pi-hole-android-private-dns/master/assets/banner.jpg"> <br/>

I came across Pi-hole about a year ago, and have been using it on and off since then for small projects.

A few months ago I decided to use it for private DNS, but the compatibility with Android Private DNS was not widely available or effective. I spent many hours searching over the internet, piecing together code from various sources and testing it.

I am finally happy to say that I am able to create a working piece of code for Android Private DNS!

As a member of the open source community, I would like to give back, and am posting the code here for use by fellow members. I am sure there are at least a few members out there who may have need for this code.

## Requirements
1. Ubuntu / Debain Based (Any Version)
2. Pi-Hole Installed With Web Server
3. Allow The Following Ports in TCP (`80,443,853`)

***Note*** I dont use Raspberry Pi to run Pi-Hole so i was not able to test. but the same steps are required for it.

## Installation
This is a simple script which requires 2 arguments
1. Domain Name To Run Android Private DNS Service
2. Email To Share with letsencrypt to get an SSL For Android Private DNS

```
sudo wget https://raw.githubusercontent.com/varunsridharan/pi-hole-android-private-dns/master/pi-hole-android-private-dns.sh
sudo bash pi-hole-android-private-dns.sh {domain_name} {email_for_letsencrypt}
```

**Example Run** `sudo bash pi-hole-android-private-dns.sh mydns.example.com myemail@gmail.com`

---


<!-- START common-footer.mustache -->
<!-- END common-footer.mustache -->