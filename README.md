####  *INTRODUCING!*
# whereall
### Swift command line utility alternative to where! 
#### very useful, in many cases, like when using xargs
#### Its blazing fast, much faster than any ol' zsh or bash function could ever. Thanks to swift!
##### *Codesigned by Apple Developer ID*

where is a *built in shell command* and doesnt have a location and xargs **only** acts upon *executables*, for instance.

```
◬ main⎪●◦◌◦⎥ py⌉⌊3.8 sw ◁ 6.2arm64 01:48
   ls  /opt/homebrew/cellar/llvm/20.1.8/bin | xargs -I {} where {}                                                                                                 
xargs: where: No such file or directory
```
```
 $ where where                                                                                                                                                    
where: shell built-in command
```
```
$ ls /opt/homebrew/cellar/llvm/20.1.8/bin | xargs -I {} ./whereall {}                                                                            

/opt/pkg-2025Q1/bin/amdgpu-arch
/opt/homebrew/opt/llvm/bin/amdgpu-arch
/opt/pkg-2025Q1/bin/analyze-build
/opt/homebrew/opt/llvm/bin/analyze-build
/opt/pkg-2025Q1/bin/bugpoint
/opt/homebrew/opt/llvm/bin/bugpoint
/opt/pkg-2025Q1/bin/c-index-test
/opt/homebrew/opt/llvm/bin/c-index-test
/opt/pkg-2025Q1/bin/clang
/opt/homebrew/opt/llvm/bin/clang
~/.swiftly/bin/clang
/usr/bin/clang
etc etc etc.
```
