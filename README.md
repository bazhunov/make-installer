
# Make-installer
Bash Script for creating a self-extracting installer from the archive


# Requirements

 - bash
 - tar
 - sed
 - xxd
 - shc (to generate a binary self-extracting installer)

# Usage

    make-intaller -h
    Script for creating a self-extracting installer from the archive
    Version: 2.0.0.0
    Usage: ./make-intaller  [ -h|--help ] | [-v|--version] | [-b|--binary] [-d|--destination <path>] <-a|--archive <tar.gz file>>
    
    -h|--help                     Display help and exit
    -v|--version                  Display version and exit
    -b|--binary                   Create a binary self-extracting installer. The 'shc' (shell script compiler) utility is required.
                                  In absence 'shc', the option will not work and self-extracting bash-installer will be created.
                                  URL: https://neurobin.org/projects/softwares/unix/shc
    -d|--destination <path>       The destination path for extracting data. Default: current directory
    -a|--archive <tar.gz file>    Source archive (file type: tar.gz )

# License
GNU General Public License v3.0