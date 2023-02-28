# whd on whd-work to doc/README3.md

Method: There are two files: README3.md and HOWTO.org. I want to keep HOWTO.org on whd-work and put README3.md on main.

I'm currently on whd-work branch

I'll do 

    % git add .
    % git commit  -m 'blah blah blah'
    % git push
    
to push to github.com. 

Unfortunately, the last step failed because I haven't set an upstream branch yet. As Git advised, I need to ...

	% git push --set-upstream origin whd-work

Then 'realize' my mistake and (I think), do 

    % git reset HEAD~1 # (would git reset HEAD^ work?)
    
This should reset the current commit to the state of the repository to just before the last commit that mistakenly put HOWTO.org on whd-work.

I'll investigate how the refs change both locally and remotely, showing examples. 

Then, do 

    % git checkout main, 
    % git add README3.md
    % git commit commit -m " ... " README3.md 
    % git push
    
then
 
    % git checkout whd-work
    % git add HOWTO.org
    % git commit -m "..." HOWTO.org 
    % git push
    
and we should be golden.    

