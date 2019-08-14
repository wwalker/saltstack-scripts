# saltstack-scripts
saltstack-scripts is a collection (currently one) of scripts written to extend saltstack features.

## salt-where
salt-where lists minions that would run a given state based on top/top.sls
salt-where [-f] <state_name>
    -f - reuse the cached data from the last run (instant vs about 1 minute)
         the cached data is from running state.show_top on each minion
Caveat - this script kicks off all the state.show_top processes at once.  I only have about 200 minions on any one salt-master, so it is not a problem.  It may be a problem on your salt master.
