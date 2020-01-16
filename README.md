# ECE 250 Test Cases
This repo is intened to host test cases for students to run against their ECE 250 projects. This does not garentee that by passing
all cases that it will pass the automarker

# Running Test Cases on Windows 10 (PowerShell)
Place the following in a .ps1 file
```
$testin=$args[0]
$testout=$args[1]
$testdriver=$args[2]
diff (cat $testin | %testdriver) (cat $testout)
```
Example running a test: 
.\runTest.ps1 test1.in test1.out .\testDriver.exe


### Owner
Quinn Hodges
