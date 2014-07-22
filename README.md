hg-clone-bash
=============

Bash Script to pull mercurial repo changeset-by-changeset

NOTE: CURRENTLY OPTIMIZED FOR mozilla-central repo. I wish to find no. of total revisions in future. 
One probable way might be `curl`ing the remote address and finding the changeset (Doesn't yet know if all the remote repo could be supported like this)

##Get it working

1. Clone the Repo,
2. go over to the directory 
3. run `./clone.sh <remote-repo-addr> <local-addr>`
4. If you cancelled the process, go to `<local-addr>` and run `./pull.sh`

#Problems

1. hg does not allow shallow clone, so we HAVE to clone every-freakin-thing
2. hg cannot pause-and-resume the clone, so ppl having low-internet-speed are sucked!


#Solution?

1. mimic the pause-and-resume scenario by pulling only some changeset at a time, saving the state and resuming.


#Still under Development. Please Contirbute or Suggest Features!

