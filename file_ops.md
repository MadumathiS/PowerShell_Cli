#    File operations

Now that we know how to move in the file system, let's check how to manipulate files and folders. In this challenge, you will discover and use the commands Get-Content, echo, New-Item, Move-Item, Copy-Item, and Remove-Item.

1. Create a file named story1.txt

2. Type echo "Hello World" > story1.txt

3. Print the content of the file
```
 echo "Hello World" > story1.txt

PS C:\Users\varad> Get-content story1.txt

Hello World
```

4. Create a folder named story

`New-Item -Path 'C:\Users\varad\story' -ItemType Directory`

` Directory: C:\Users\varad`

`Mode                 LastWriteTime         Length Name`
----                 -------------         ------ ----
`d-----        28-04-2022     13:31                story`


5. Move story1.txt inside story

`Move-Item C:\Users\varad\story1.txt C:\Users\varad\story`

6. Copy story1.txt as story2.txt


`PS C:\Users\varad\story> Copy-Item 'story1.txt' 'story2.txt'`
`PS C:\Users\varad\story> ls`
` Directory: C:\Users\varad\story`


`Mode                 LastWriteTime         Length Name`
`----                 -------------         ------ ----`
`-a----        28-04-2022     11:11             28 story1.txt`
`-a----        28-04-2022     11:11             28 story2.txt`

7. Print both files

`PS C:\Users\varad\story> Get-Content story1.txt`
`Hello World`

`PS C:\Users\varad\story> Get-Content story2.txt`
`Hello World`

8. Rename story2.txt as me.txt

`PS C:\Users\varad\story> Rename-Item story2.txt me.txt`
`PS C:\Users\varad\story> ls`
` Directory: C:\Users\varad\story`
`Mode                 LastWriteTime         Length Name`
`----                 -------------         ------ ----`
`-a----        28-04-2022     11:11             28 me.txt`
`-a----        28-04-2022     11:11             28 story1.txt`

9. Append me.txt and add "I am a junior at Becode"

`PS C:\Users\varad\story> Add-Content me.txt 'I am a Junior at Becode'`
`PS C:\Users\varad\story> Get-Content me.txt`
`Hello World`
`I am a Junior at Becode'`

10. Remove the folder story with it's content
` Remove-Item story`



