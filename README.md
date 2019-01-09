# ami-jars
point releases of ami executables (normally as maven-appassembler jar-with-dependencies)

## structure
Releases are named with the date (e.g. `ami20190109`). Each is a directory with two subdirectories `bin` and `repo` created by the Maven 
`appassembler` plugi. The structure is:
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
