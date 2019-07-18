# Euro Checksum

Euro (€) is the currency of the euro area and has been in circulation since 2002. The banknotes of the euro are issued by the national central banks of the Eurosystem or the European Central Bank.  
The euro notes contain many complex security features such as serial number, watermarks, invisible ink characteristics, holograms, optically variable inks and microprinting that document their authenticity.  
There are two series of euro banknotes:
- 1st series issued from 2002;
- 2st series or Europa series issued 2013.

## Checksum
Each note has a unique serial number of 12 characters:
- 1st series notes have a letter as first character (that specifies the country of issue) and 11 digits;
- 2st series notes have a letter as first character such as 1st series, but 10 digits because the second char is also letter in order to increment combinations.

Each country (i.e. first char) has a control code (for example the letter of Italy is 'S' and its control code is 7) and the sum of all digits and the ASCII of the second letter for Europa series until the result is less than 9 (i.e. the root), must be equals to control code in order to pass the checksum.  
*Example:*
- *SA2160296285 is the serial number;*
- *'S' specifies the country and, particularly, Italy with control code equals to 7;*
- *the ASCII of A is 65;*
- *the sum is: 6+5+2+1+6+0+2+9+6+2+8+5=52 -> 5+2=7*
- *the obtained root coincides with the control code.*

Tables of control codes at [Wikipedia page](https://en.wikipedia.org/wiki/Euro_banknotes).