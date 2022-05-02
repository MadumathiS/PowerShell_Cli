# Get-Help


  GET-HELP
    The Get-Help cmdlet displays help at the command line from content in help files on your computer. Without help files, Get-Help displays basic help about cmdlets and functions. You can also use Get-Help to display online help for cmdlets and functions.
```
    To get help for a cmdlet, type:        Get-Help <cmdlet-name>

    To get online help, type:        Get-Help <cmdlet-name> -Online

    The titles of conceptual topics begin with "About_".
     To get help for a concept or language element, type:
     `  Get-Help About_<topic-name>`
    To search for a word or phrase in all help files, type:
        Get-Help <search-term>

    For more information about the Get-Help cmdlet, type:

        Get-Help Get-Help -Online

    or go to: http://go.microsoft.com/fwlink/?LinkID=113316
```
```
  EXAMPLES:
      Save-Help              : Download help files from the Internet and saves
                               them on a file share.
      Update-Help            : Downloads and installs help files from the
                               Internet or a file share.
      Get-Help Get-Process   : Displays help about the Get-Process cmdlet.
      Get-Help Get-Process -Online
                             : Opens online help for the Get-Process cmdlet.
      Help Get-Process       : Displays help about Get-Process one page at a time.
      Get-Process -?         : Displays help about the Get-Process cmdlet.
      Get-Help About_Modules : Displays help about Windows PowerShell modules.
      Get-Help remoting      : Searches the help topics for the word "remoting."
      

  SEE ALSO:
      about_Updatable_Help
      Get-Help
      Save-Help
      Update-Help

```
