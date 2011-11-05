#phpdien

A simple PHP development server using lighttpd. 

##Requirements

You will need a UNIX or UNIX-like operating system with bash. You will also need lighttpd and php5-cgi.

If you don't have them or are not sure, getting them in Ubuntu or Debian is easy. It's as simple as running:

`sudo apt-get install lighttpd php5-cgi`

The lighttpd.conf file embedded in the phpdien script was written with Ubuntu in mind, so you may have to modify it slightly to get it to work for your system. It will probably be a good idea in the future to separate it and make it configurable outside of the script.

##Installation

After you have installed the required dependencies, clone the repository and copy the phpdien script to either the root directory of your PHP project, or in /usr/local/bin or equivalent. It doesn't really matter that much.

You will also need to make the script executable, which you can do like so:

`chmod +x phpdien`

##Usage

Run phpdien from the *root* of your PHP project. This is extremely important if you want it to run correctly.

When the server starts, you may access it at: http://localhost:8000

If you want to change the port number, you must change the script.
