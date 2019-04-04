
# Pacman Commands

## Searching

Querying package databases:

Pacman can search for packages in the database, searching both in packages' names and descriptions:
$ pacman -Ss string1 string2 ...

Sometimes, -s's builtin ERE (Extended Regular Expressions) can cause a lot of unwanted results, so it has to be limited to match the package name only; not the description nor any other field:
$ pacman -Ss '^vim-'

To search for already installed packages:

$ pacman -Qs string1 string2 ...

To search for package file names in remote packages:

$ pacman -Fs string1 string2 ...

To display extensive information about a given package:

$ pacman -Si package_name

For locally installed packages:

$ pacman -Qi package_name

Passing two -i flags will also display the list of backup files and their modification states:

$ pacman -Qii package_name

To retrieve a list of the files installed by a package:

$ pacman -Ql package_name

To retrieve a list of the files installed by a remote package:

$ pacman -Fl package_name

To verify the presence of the files installed by a package:

$ pacman -Qk package_name

Passing the k flag twice will perform a more thorough check.

To query the database to know which package a file in the file system belongs to:

$ pacman -Qo /path/to/file_name

To query the database to know which remote package a file belongs to:

$ pacman -Fo /path/to/file_name

To list all packages no longer required as dependencies (orphans):

$ pacman -Qdt
Tip: Add the above command to a pacman post-transaction hook to be notified if a transaction orphaned a package. This can be useful for being notified when a package has been dropped from a repository, since any dropped package will also be orphaned on a local installation (unless it was explicitly installed). To avoid any "failed to execute command" errors when no orphans are found, use the following command for Exec in your hook: /usr/bin/bash -c "/usr/bin/pacman -Qtd || /usr/bin/echo '=> None found.'"
To list all packages explicitly installed and not required as dependencies:

$ pacman -Qet

Find the locations of installed files of a package:

pacman -Ql <package name> 

## Cache Cleaning 

 To remove all the cached packages that are not currently installed, and the unused sync database, execute:

 pacman -Sc

To remove all files from the cache, use the clean switch twice,and leave nothing in the cache folder:

 pacman -Scc

 Delete all cached versions of installed and uninstalled packages, except for the most recent 3, by default:

 paccache -r

 Define how many recent versions you want to keep. To retain only one past version use:

 paccache -rk1

## Pactree
To view the dependency tree of a package:

$ pactree package_name

## Debug 

pacman -Sy --debug 
