# CMD Guardian

![guardian](https://user-images.githubusercontent.com/84273110/183107893-45e2d5d6-ef47-4304-b9f3-72b1dced6276.png)

CMD Guardian was initially written to prank my co-workers, but it can also be used for educational purposes. It demonstrates some living-off-the-land techniques that are often used by read-world attackers:

* Persistence via Image File Execution Options
* Fileless VBScript execution using rundll32 and mshtml.dll
* Storing files in the registry
* A self-deleting `.vbs` file
* Decoding Base64 using CertUtil
* Malicious `.hta` files

## Warning

CMD Guardian is **potentially harmful**, and should only be installed in a safe and isolated environment, as if it were actual malware.

## Installation

**Disable Windows Defender before the installation**

Windows Defender flags and blocks the persistence mechanism used by CMD Guardian, and rightfully so. It reactivates itself after being switched-off, so be sure to [disable it permanently](https://www.alphr.com/disable-windows-defender-windows-11/). Alternatively, you can install CMD Guardian on a Windows 7 machine, and avoid this hassle altogether.

To install CMD Guardian, simply execute the `guardian.reg` file. Then, open a command prompt and see what happens!

## Limitations

CMD Guardian was tested on Windows 7, Windows 10 and Windows 11. It doesn't work on Windows XP.

## License

[MIT](https://choosealicense.com/licenses/mit/)

