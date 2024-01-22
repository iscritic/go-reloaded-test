# go-reloded-test
This is a fork of the [go-reloaded_test](https://github.com/saveAsPerfect/go-reloaded_test) project.

## Objectives
go-reload-test is automatic tester for go-reload project.

## How to use

- Place the contents in the root folder of the program:
```
├── TestCases/
│   ├──case1.txt
│   └── ...
├── YourOutput/
├── ExpectedOutput/
|   ├──case1_expected.txt
│   └── ...
│  
├── main.go
├── go.mod
└── script.sh

```
Change the permissions to make the script executable and run.
```
$chmod +x script.sh
$./script.sh
```

Failed cases will be displayed in red, with `your output` on top and the `expected` one below it
```
< AN book an apple a dog
\ No newline at end of file
---
> A book an apple a dog
\ No newline at end of file
```

## Go directories

### `/TestCases` 
All test cases are stored in this folder 

### `/ExpectedOutput`
Expected output for `TestCases`, pay atentions to the `\n` newlines at the end of the file

### `/YourOutput`
This is your output

## Notes
You can create your own test cases following the original