
# Born Again Shell (bash)

# Why use bash script?

It makes the things easier and more automated.

## Simple script
`[train@localhost play]$ nano simple.sh`

#!/bin/bash  
echo "I am a simple bash script"
```
[train@localhost play]$ sudo chmod +x simple.sh
[sudo] password for train:
[train@localhost play]$ ./simple.sh
I am a simple bash script
```

### If we are in the same directory with the script file to run we use ./, bash, sh ..  

## Shells
- Always start with to tell OS which shell to use  
 List available shells  
 ```
 [train@localhost play]$ cat /etc/shells
/bin/sh
/bin/bash
/usr/bin/sh
/usr/bin/bash
/bin/tcsh
/bin/csh
```

## Shebang
` #!/bin/bash – Execute the file using the Bash shell `

```
#!/bin/sh – Execute the file using the Bourne shell, or a compatible shell, assumed to be in the /bin directory
#!/bin/bash – Execute the file using the Bash shell
#!/usr/bin/env python3 – Execute with a Python interpreter, using the env program search path to find it
#!/bin/false – Do nothing, but return a non-zero exit status, indicating failure.
```

## Which shell does use my user?
```
cat /etc/passwd | grep train
train:x:1000:1000:train:/home/train:/bin/bash
```

