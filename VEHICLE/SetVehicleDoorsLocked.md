---
ns: VEHICLE
---
## SET_VEHICLE_DOORS_LOCKED

```c
// 0xB664292EAECF7FA6 0x4CDD35D0
void SET_VEHICLE_DOORS_LOCKED(Vehicle vehicle, int doorLockStatus);
```

```
1 - can get in, can leave
2 - CARLOCK_LOCKED (can't get in, can leave)  
3   car is being ignored when trying to enter, can leave
4 - CARLOCK_LOCKED_PLAYER_INSIDE (tries to open it, but it is locked, then getting in with breaking the window, can't leave)  
(maybe, these are leftovers from GTA:VC)  
5 - can get in, can leave
6 - can get in, can leave
7 - can get in with breaking the window, 
(source: GTA VC miss2 leak, matching constants for 0/2/4, testing)  
They use 10 in am_mp_property_int, don't know what it does atm.  
```

## Parameters
* **vehicle**: 
* **doorLockStatus**: 

