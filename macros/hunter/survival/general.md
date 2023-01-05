
## Survival Hunter Macros:

#### 434 Explosive shot Macro:

> **Note:** What is 4,3,4?
It’s been found that rank 3 and 4 of explosive shot don’t overwrite each other
When lock n load procs 
You cast rank 4(max rank) explosive shot 
Then immediately cast rank 3 explosive shot 
Then immediately cast rank 4 of explosive shot 
The ticks don’t cancel each other

> By making explosive shot get on cd sooner you can squeeze out one more es per minute leading to ABOUT A 120 dps gain (on the assumption you get 2 LNL per min) 

> Is this bugged and will it get fixed? Time will tell
Do you need to have this macroed? No
If you wish to have 4,3,4 macroed here is a provided
Can i add other things to that macro? Yes
Can this macro be used outside of LNL? Yes 


```
/castsequence reset=2,target Explosive Shot,Explosive Shot(Rank 3)
```


> **Note:** Can I spam my ES macro if I have that castsequence? YES
With the reset=2,target the sequence will reset to ES(Rank4) before ES comes off cooldown or if you are tab-targetting to multiple mobs to apply ES to 2/3 mobs during a LnL proc, it will reset the sequence each time the target changes.