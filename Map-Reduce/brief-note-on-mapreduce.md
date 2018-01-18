**Map Reduce**

Map reduce is a programming framework for programming, that is applied to the data in the data node. This is a Tiger approach, since the code is applied to the data.

There are 3 steps in map reduce:

    1.Step 1 - **Mapper Phase** :  
        
        a).Generation of Key-value pairs.
        b).I/O operation takes place here.
        
    2.Step 2 - **Sort & Shuffle Phase** :  
    
        a).We dont need to write code to perform this step, Hadoop performs this on its own.
        b).Network transfer of data and I/O operations takes place here.
        
    3.Step 3 - **Reducer Phase**:  
    
        a).I/O Operation takes place here.
        b).Sum the values for same keys and produce the output.
        
        
![alt text] (https://github.com/SaravananJaichandar/Big-Data/blob/master/Map-Reduce/mapreducediagram.jpg)        


**Additional Step**

**Combiner Approach**:

Performing the sort & shuffle and reducer steps on each block in the mapper phase. By this, we can reduce the networktransfer of data.
