# Makefile Manpage Project

This project is made by AdamAarbouba. It adds a simple, fully functional man page for `makefile` so you can use `man makefile` on your system.

It includes basic tips and instructions on how to install and use the man page.

## Installation


```bash
sudo mkdir -p /usr/local/share/man/man1           #1. Create the man directory if it doesn’t exist
sudo cp makefile.1 /usr/local/share/man/man1/     #2. Copy the man page file
sudo mandb                                        #3. Update the man database (optional):
man makefile                                      #4. Use it by running
groff -T ascii -man makefile.1 | less             #5. Preview without installing
