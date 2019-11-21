
# Github 

 add a existing repository to github:

 git remote add origin git@github.com:rkcb/fed.git
 git push -u origin master	

# Repository 

- show remote url => git config --get remote.origin.url

# Misc

Copy file(s) from another branch:
	git checkout <branch> -- <file(s)>

Compare branches by commits
	git log <branch> --not master --stat

To stop tracking a file that is currently tracked, use 
	git rm --cached.
