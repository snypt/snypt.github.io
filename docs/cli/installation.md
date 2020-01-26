# Installation

Check if Snypt is installed

```
snypt -v
0.1.0
```
### Install via NPM

```
npm install snypt-cl -global
```

### MacOs
Download Snypt executable from [here]() and copy the executable to a directory in your path, or any directory that will be added to your path:
```
curl -Lo bit https://github.com/teambit/bit/releases/download/v14.7.2/bit-bin-macos  
chmod +x bit
sudo cp bit /usr/local/bin/  
rm bit
```

### Windows
Download Snypt executable .exe file from [here]() then add it to your PATH:

Let's say your __snypt.exe__ file is located at **C:\myfolder\snypt.exe**

You can either manually add **C:\myfolder** to the end of your PATH Env Variable in under 
System Properties or run the following command 
 
```
set PATH=%PATH%;C:\myfolder
```

### Unix
Download Snypt executable from [here]() and copy the executable to a directory in your path, or any directory that will be added to your path:

 
```
curl -Lo bit https://github.com/teambit/bit/releases/download/v14.7.2/bit-bin-linux
chmod +x bit
sudo cp bit /usr/local/bin/  
rm bit
```

### Configure Snypt CLI

After installing the Snypt CLI, you are ready to configure your project directory and the Snypt CLI by running snypt init 
from the root directory of your project.

```
snypt init
```

This will add a snypt.json to your project containing your configuration. Snypt CLI works 
by parsing through your project and finding snypts ([more info here](/docs/cli/pushing_snypts.md)). Snypt.json
contains a list files Snypt CLI will parse through in search of snypts. 

You can add one or more files to that list by running the command

```
snypt add './app/js/file.js' './app/js/file2.js' './app/js/file3.js'
```
