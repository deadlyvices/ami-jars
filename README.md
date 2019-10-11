# ami-jars
point releases of ami executables (normally as maven-appassembler jar-with-dependencies)

## directories
Releases are named with the date (e.g. `ami20190109`). Each is a directory with two subdirectories `bin` and `repo` created by the Maven 
`appassembler` plugin and also a single `jar-with-dependencies`. (These are alternative ways of running the software). The `appassembler` method is more customised as it deals with classpaths, etc.

### appassembler 
Create a suitable software directory (e.g. `mysoftware` or in `/usr/bin`) on you machine and clone the repository into it. Your structure will be as below (`bin` and `repo`). You will be running scripts from the `bin` directory. 
You will need to set your PATH (not CLASSPATH) to the `bin` directory, e.g. on UNIX/MacOSX:
```
export PATH="/Users/pm286/mysoftware/ami20190109/bin:$PATH"
```
Test this with 
```
which ami-pdf
```
If the path points correctly then you should see a pathname. If not there will be an error message.
Now you can run the program:
```
ami-pdf
```
which should give you a help message. Further details are in the `ami` documentation






### structure
The structure is:
```
ami20190109/
```
// these are the `ami` commands. They are in pairs (Unix/Macosx, and Windows (`*.bat`)). 
This list will change in future to have more commands
```
├── bin
│   ├── ami-all
│   ├── ami-all.bat
│   ├── ami-bitmap
│   ├── ami-bitmap.bat
│   ├── ami-clean
│   ├── ami-clean.bat
│   ├── ami-dictionaries
│   ├── ami-dictionaries.bat
│   ├── ami-frequencies
│   ├── ami-frequencies.bat
│   ├── ami-gene
│   ├── ami-gene.bat
│   ├── ami-identifier
│   ├── ami-identifier.bat
│   ├── ami-image
│   ├── ami-image-old
│   ├── ami-image-old.bat
│   ├── ami-image.bat
│   ├── ami-makeproject
│   ├── ami-makeproject.bat
│   ├── ami-ocr
│   ├── ami-ocr.bat
│   ├── ami-pdf
│   ├── ami-pdf-old
│   ├── ami-pdf-old.bat
│   ├── ami-pdf.bat
│   ├── ami-pixel
│   ├── ami-pixel.bat
│   ├── ami-regex
│   ├── ami-regex.bat
│   ├── ami-search
│   ├── ami-search-cooccur
│   ├── ami-search-cooccur.bat
│   ├── ami-search.bat
│   ├── ami-sequence
│   ├── ami-sequence.bat
│   ├── ami-species
│   ├── ami-species.bat
│   ├── ami-word
│   ├── ami-word.bat
│   ├── ami-xml
│   ├── ami-xml.bat
│   ├── cmine
│   ├── cmine.bat
│   ├── contentMine
│   ├── contentMine.bat
│   ├── cproject
│   ├── cproject.bat
│   ├── makeProject
│   ├── makeProject.bat
│   ├── norma
│   └── norma.bat
```
// these are 3rd party jars which AMI needs. 
```
└── repo 
    ├── Saxon-HE-9.6.0-3.jar
    ├── activation-1.1.1.jar
    ├── asm-1.0.2.jar
    ├── asm-3.3.1.jar
    ├── boofcv-calibration-0.32.jar
    ├── boofcv-core-0.32.jar
... 
```
