# go-shellcode-helper

- Copy from https://github.com/Ne0nd0g/go-shellcode
- Edit every shellcode runner method to function for ease to import
    - Only Changed method that only requires shellcode
    - Methods such as CreateRemoteThread that needs pid is not changed

- Usage

```golang

func main() {

    shellcode, _ := hex.DecodeString("505152535657556A605A6863616C6354594883EC2865488B32488B7618488B761048AD488B30488B7E3003573C8B5C17288B741F204801FE8B541F240FB72C178D5202AD813C0757696E4575EF8B741F1C4801FE8B34AE4801F799FFD74883C4305D5F5E5B5A5958C3")
    CreateProcess.Run(shellcode)

}


```