# Try #2

I got into a *terrible* mess trying to make 2 changes while on /whd-work/, one to this file and one to HOWTO.org, then commit and push to the remote tracking branch of /whd-work/.

Then, switch back to /main/, realize my mistake that I didn't want the changes I'd made on HOWTO.org /whd-work/, but on /main/.

So, I *thought* I'd do the following

1. Rebase whd-work back to the state *before* I'd done the commit
2. Switch to /main/
3. commit HOWTO.org; push to remote
4. Switch back to /whd-work/
5. commit README3.org; push to remote.
