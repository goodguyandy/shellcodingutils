# shellcodingutils
some utils I use during shellcode development

## shellcodeextract.sh 

a  shellcode extractor that prints on the stdout the opcodes and does some error checking 

usage:
```console
./extractshellcode.sh bulletproof
---------- opcodes -------
"\x90\x50\x90\x50\x90\x50\x90\x50\x90\x50\x90\x50\x90\x50\x90\x50\x31\xc0\xb0\x01\x31\xdb\xb3\x10\xcd\x80\xfc\xbb\xff\x00\x00\x00\x66\x81\xc9\xff\x0f\x31\xd2\x41\x31\xc0\xb0\x43\xcd\x80\x3c\xf2\x74\xe8\xb8\x90\x50\x90\x50\x89\xcf\xaf\x75\xeb\xaf\x75\xe8\xff\xe7"
--------------------------
attention, null byte found:
"\x90\x50\x90\x50\x90\x50\x90\x50\x90\x50\x90\x50\x90\x50\x90\x50\x31\xc0\xb0\x01\x31\xdb\xb3\x10\xcd\x80\xfc\xbb\xff\x00\x00\x00\x66\x81\xc9\xff\x0f\x31\xd2\x41\x31\xc0\xb0\x43\xcd\x80\x3c\xf2\x74\xe8\xb8\x90\x50\x90\x50\x89\xcf\xaf\x75\xeb\xaf\x75\xe8\xff\xe7"
--------
 804807b:	bb ff 00 00 00       	mov    ebx,0xff
```
