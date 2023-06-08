#Shell Permissions
These are shell permissions. I don't get why the linuxcommand.org has to be so cruel.
Giving values of:
rwx as 7
rw- as 6
r-x as 5
r-- as 4


##What would be easier
THey could've just said:
Value of r is 4
Value of w is 2
Value of x is 1
Value of - is 0


###Calculating numerical value of permissions
For each group of three, add their values.
For example:
	r-xr--r--
	take each three characters for owner, group owner & others respectively:
			r-x | r-- | r--
			4+0+1 | 4+0+0 | 4+0+0
			5 | 4 | 4

		numerical value = 544
		(I used the pipes(|) to brea the permissions into groups of 3. A - before permissions would also mean a regular file.)
