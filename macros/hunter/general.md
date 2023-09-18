## General Hunter Macros

#### Cooldown Macro w/ Everything in it:

> **Note:** "13" and "14" refer to the two trinket slots respectively, while 10 refers to gloves. Remove as necessary or keep it to not be forgotten.
"/cqs" refers to cancelling queued spells.

```
#showtooltip Rapid Fire
/cast Kill Command
/use [harm] Furious Howl
/use [harm] Rabid
/cast Rapid Fire
/use [combat] 10
/use [combat] 13
/use [combat] 14
/use [harm] Call of the Wild
/cqs
```

#### All-In-One Pet Heal & Call Macro:
```
#showtooltip
/use [@pet,nodead,exists] Mend Pet
/stopmacro [@pet,nodead,exists]
/use [@pet,dead,exists] Revive Pet
/castsequence reset=1.5 Call Pet, Revive Pet
```

#### Misdirection Macro:

> **Note:** Lets you use Misdirection easily on mouse-over, focus, target, or your pet based on whether you have a mouse-over target, a focus, or just your pet.  I highly recommend to use it always with focus target, but this macro keep it flexible. 
Priority = Mouse-Over > Focus Target > target > Your Pet

```
#showtooltip
/cast [@mouseover,help][@focus,help][help][@pet,exists][] Misdirection
```

#### Cursor Flare/Volley Macro:

> **Note:** Replace <Flare or Volley here based on choice> with Volley / Flare.

```
#showtooltip
/cast [@cursor] <Flare or Volley here based on choice>
```

#### Pet Attack Macro:

```
#showtooltip
/cleartarget [dead][help]
/targetenemy [noexists,combat]
/use [nopet] Call Pet
/use [nochanneling,harm] Kill Command
/petattack [@mouseover,harm][@target,harm] [@pettarget,exists]
/use [harm] Dash
/petautocastoff [group] Growl
```

#### Pet Passive Macro:

```
/petpassive
/petstay [mod]
/petfollow [nomod]
```

#### Steam Tonk + Dream Vision Macro:

```
#show
/use [nopet] Call Pet
/cancelaura Steam Tonk Controller
/use [nocombat,pet] Steam Tonk Controller
/cancelaura Dream Vision
/use [combat,pet] Elixir of Dream Vision
/cast [combat,pet] Dismiss Pet
/use [nopet] Call Pet
```

### Master's call

```
/petpassive [nomod]
/petfollow [nomod]
/petpassive
/use [combat,nomod] Dash
/use [@player]Master's Call
/petautocastoff Call of the Wild
/petautocastoff Dash
/petautocastoff [group] Growl
/petautocaston [nogroup] Growl
```

#### Kill Shot mouse over 

```
/use [@mouseover,harm][]Kill Shot
```

#### Serpent sting mouse over

```
/use [@mouseover,harm][]Serpent Sting
```

#### Aspect weaving Macro:

> **Note:** Allows you to switch between Dragonhawk and Viper, which is very usefull if you want to recover mana in the mid-encounter. Notice that while in Aspect of Viper, if you use another aspect in between, you need to press this macro twice to switch back to Dragonhawk.

```
#showtooltip Aspect of the Dragonhawk
/castsequence Aspect of the Dragonhawk, Aspect of the Viper
```

#### Trap weaving Macro:

> **Note:** "41119" and "42641" refer to the saronite bomb and global thermal saper charge respectively.
> - [group:raid,combat,harm] allows the Global Thermal Saper Charge to only be cast in raid groups if you are in combat and you have a target that is an enemy, to not be too much expensive. Make sure you also have another key binding to "trap weave" without Global Thermal Saper Charge, if you don't want to use it on trash. 
> - [@player,combat] allows the Saronite Bomb to be cast in yourself if you are in combat.

```
#showtooltip Explosive Trap
/use [@pettarget,exists,combat][@player,combat]Furious Howl
/use [group:raid,combat,harm]item:42641
/use [@player,combat]item:41119
/use [combat,harm]Raptor Strike
/use Explosive Trap
```



