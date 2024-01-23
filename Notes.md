## 1. Set up environment (Software) 
go to https://github.com/abstracthat/dactyl-manuform and follow the steps to generate design
1. [Install the Clojure runtime](https://clojure.org/)
2. [Install the Leiningen project manager](https://leiningen.org/)
   1. Installation for Windows
      1. download [lein.bat](https://raw.githubusercontent.com/technomancy/leiningen/stable/bin/lein.bat)
      2. it will be download as txt file, open it with text editor and do "save as" new file name "lein.bat", remember to update the file extension to be *
      3. run the bat file via CMD by simply type in the file name "lein.bat" when you are in the directory. for detailed guide to work with bat file, see [bat guide](https://www.makeuseof.com/tag/write-simple-batch-bat-file/#:~:text=Save%20as%20BAT%20File,will%20finalize%20the%20batch%20process.)
         1. I firstly got result 
         ```
         C:\Path\.lein\self-installs\leiningen-2.10.0-standalone.jar can not be found.
         You can try running "lein self-install"
         or change LEIN_JAR environment variable
         or edit lein.bat to set appropriate LEIN_JAR path.
         ```
         2. follow the guide to enter and run `lein self-install` which will start downloading Leiningen
         3. after it is finished, run the bat by enter and run "lein.bat" again, I got the following result
         ```
         C:\PATH\Downloads>lein.bat
         Leiningen is a tool for working with Clojure projects.
 
         Several tasks are available:
         change              Rewrite project.clj with f applied to the value at key-or-path.
         check               Check syntax and warn on reflection.
         classpath           Write the classpath of the current project to output-file.
         clean               Removes all files from paths in clean-targets for a project
         compile             Compile Clojure source into .class files.

         and more
         ```
    2. Run it in Windows
       1. PROBLEM: could not find lein when I try to run `lein generate` in the repo
          - Reason: lein isn't recognized by cmd due to it is not in the PATH to be accessed anywhere
          - Answer: install it again in the place we need it by copying the lein.bat file to the repo and run `lein` in the cmd again to install it
3. [Install OpenSCAD]()