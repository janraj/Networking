# Problem 
   You have a cluster of 10000 machines with commodity disks. Each machine has thousands of arbitrary sized files upto 3GB named distinctly per machine. You need to dedup or replicate the files across the cluster by content & name. Each file with the same content and name should be present on at least  three separate machines across three separate racks and no more. You can assume the files list are static and there is enough space to accommodate all copies of all files in the cluster.

# Goal 
    Build a distributed deduplication and replication system 

# Functional Requirement 
    1. Uniquely identify file 
    2. Exisit on exactly three machin eeach on different rack 
    3. Never exisit more than 3 times
    4. never exisit on the same rack more than once 

# Non functional requirements 
    1. Performance 

# Detailed Design 
    identify duplicates across cluster, ensure exactly 3 distinct copies exist. 
    1. We need to build file identifier 
    2. Metadata collection phase 
    3. Create global map

## Map reduce style pseudocode
    Each machine contains a lits of files , files are static.  We need exactly 3 copies of each file stored pn 3 different machines each ina different rack. Deduplicate where there are more than 3 
### mapper 
   1. each machine emits meta data for its files 
   2. Shullfle and sort 
   3. Reducer 
   4. Execution Engine 


