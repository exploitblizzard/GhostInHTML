# GhostInHTML

Usage
----------------------

**Youtube : https://youtu.be/ozjyrSS4jWo**

Few payload examples files are provided in the `payloads_examples` directory. For instance the `calc.xll` is an Excel add-in (XLL) file that contains a metasploit shellcode for x86 processes to launch the `calc.exe` process.

**Using the python script**

1/ Generate the malicious html file from the XLL file, along with a secret key:
`python embedInHTML.py -k mysecretkey -f example_calc.xll -o index.html`

2/ Expose the html file on a web server (*one can be optionnaly started for you with the `-w` flag*)
