# saltstack-scripts
saltstack-scripts is a collection (currently one) of scripts written to extend saltstack features.

## salt-where
salt-where lists minions that would run a given state based on top/top.sls
salt-where [-f] <state_name>
    -f - reuse the cached data from the last run (instant vs about 1 minute)
         the cached data is from running state.show_top on each minion

