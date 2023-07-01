
 
# How to Find and Update Your Matlab R2009a License File
 
If you are using Matlab R2009a on a network license, you might need to find or update your license file for various reasons. For example, if you change the license server name, port number, or add new products to your license. In this article, we will show you how to locate and modify your license file on different operating systems.
 
**Download File ✸ [https://t.co/u2QZHZBezS](https://t.co/u2QZHZBezS)**


 
## Where to Find Your License File
 
The location of your license file depends on your license type and operating system. The license file is a specially formatted ASCII text file that contains encrypted product passcodes for each product you are licensed to run. Each product passcode identifies the number of keys available for that product[^1^].
 
For individual licenses, the license file is stored in a hidden folder within your home folder. For designated computer, concurrent, and network named user licenses, the license file is stored in the "licenses" folder within the Matlab installation folder[^1^]. Here are some examples of where to find your license file on different operating systems:
 
- Windows: Individual licenses are stored in `%AppData%\MathWorks\MATLAB\R2009a_licenses`. Network licenses are stored in `C:\Program Files\MATLAB\R2009a\licenses`.
- MacOS: Individual licenses are stored in `/Users/$USER/Library/Application Support/MathWorks/MATLAB/R2009a_licenses`. Network licenses are stored inside the Matlab application package. Right click, CTRL-click, or two-finger click on the Matlab icon in your Applications folder and select "Show Package Contents". In the folder that opens up, open the "licenses" folder.
- Linux: Individual licenses are stored in `~/.matlab/R2009a_licenses`. Network licenses are stored in `$MATLAB/licenses`.

## How to Update Your License File
 
If you need to update your license file, you can do so by editing the text file with a text editor. However, you should only edit the license file if you know what you are doing and have a backup copy of the original file. Some common reasons to edit the license file are:

- Changing the license server name or port number: You need to edit the SERVER line in the license file to reflect the new server name or port number. The SERVER line identifies the server host and port number[^2^]. For example, if your new server name is "myserver" and port number is "27000", you need to change the SERVER line to `SERVER myserver ANY 27000`.
- Adding new products to your license: You need to add new INCREMENT lines to the license file for each new product you want to run. The INCREMENT line identifies a product, the number of keys available for the product, and other information[^2^]. For example, if you want to add Simulink to your license, you need to add an INCREMENT line like this: `INCREMENT SIMULINK MLM 46 30-jan-2025 1 7DE4D05FF067 VENDOR_STRING=vi=0:at=200:ae=1:lu=300:lo=CN:ei=1234567:lr=1:2p=0:DUP_GROUP=UH asset_info=123456 ISSUED=21-Nov-2021 BORROW=720 NOTICE=product=SIMULINK SN=123456 SIGN="00BE C534 0A32 1821 AFCE D040 2085 3E00 9005 4983 7EFB 875F E4A7 FEE6 9548"`. You can get the INCREMENT lines for your new products from MathWorks Support or from your license administrator.

After editing your license file, you need to restart the network license manager on the server and restart Matlab on the client machines for the changes to take effect.
 
## Conclusion
 
In this article, we have shown you how to find and update your Matlab R2009a license file on different operating systems.
 8cf37b1e13
 
