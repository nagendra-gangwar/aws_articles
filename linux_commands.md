# copy a file 

option	description

cp -a	archive files 

cp -f	force copy by removing the destination file if needed 

cp -i	interactive - ask before overwrite

cp -l	link files instead of copy

cp -L	follow symbolic links

cp -n	no file overwrite

cp -R	recursive copy (including hidden files)

cp -u	update - copy when source is newer than dest


cp -v	verbose - print informative messages


Example:- 
cp source destination

# search all files in a directory for a specified text

find ./ -type f -name "*.txt" -exec grep 'test to search'  {} \;

# display disk free 

df -ha

# disk space taken by all the dir

du -sh <dir>
