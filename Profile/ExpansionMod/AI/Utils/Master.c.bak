class Expansion_Vehicles_GoToVehicle_State_0 extends ExpansionState_GoToVehicle {
Expansion_Vehicles_FSM_0 fsm;
void Expansion_Vehicles_GoToVehicle_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Vehicles_GoToVehicle_State_0";
m_Name = "GoToVehicle";
}
override void OnEntry(string Event, ExpansionState From) {
super.OnEntry(Event, From);
entity = fsm.entity;	
seat = fsm.seat;
super.OnEntry(Event, From);	
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
super.OnExit(Event, Aborted, To);
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
if (super.OnUpdate(DeltaTime, SimulationPrecision) == EXIT) return EXIT;
return CONTINUE;
}
}
class Expansion_Vehicles_GetInVehicle_State_0 extends ExpansionState_GetInVehicle {
Expansion_Vehicles_FSM_0 fsm;
void Expansion_Vehicles_GetInVehicle_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Vehicles_GetInVehicle_State_0";
m_Name = "GetInVehicle";
}
override void OnEntry(string Event, ExpansionState From) {
super.OnEntry(Event, From);
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
super.OnExit(Event, Aborted, To);
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
if (super.OnUpdate(DeltaTime, SimulationPrecision) == EXIT) return EXIT;
return CONTINUE;
}
}
class Expansion_Vehicles_GetOutVehicle_State_0 extends ExpansionState_GetOutVehicle {
Expansion_Vehicles_FSM_0 fsm;
void Expansion_Vehicles_GetOutVehicle_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Vehicles_GetOutVehicle_State_0";
m_Name = "GetOutVehicle";
}
override void OnEntry(string Event, ExpansionState From) {
super.OnEntry(Event, From);
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
super.OnExit(Event, Aborted, To);
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
if (super.OnUpdate(DeltaTime, SimulationPrecision) == EXIT) return EXIT;
return CONTINUE;
}
}
class Expansion_Vehicles_OpenVehicleDoor_State_0 extends ExpansionState_OpenVehicleDoor {
Expansion_Vehicles_FSM_0 fsm;
void Expansion_Vehicles_OpenVehicleDoor_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Vehicles_OpenVehicleDoor_State_0";
m_Name = "OpenVehicleDoor";
}
override void OnEntry(string Event, ExpansionState From) {
super.OnEntry(Event, From);
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
super.OnExit(Event, Aborted, To);
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
if (super.OnUpdate(DeltaTime, SimulationPrecision) == EXIT) return EXIT;
return CONTINUE;
}
}
class Expansion_Vehicles_CloseVehicleDoor_State_0 extends ExpansionState_CloseVehicleDoor {
Expansion_Vehicles_FSM_0 fsm;
void Expansion_Vehicles_CloseVehicleDoor_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Vehicles_CloseVehicleDoor_State_0";
m_Name = "CloseVehicleDoor";
}
override void OnEntry(string Event, ExpansionState From) {
super.OnEntry(Event, From);
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
super.OnExit(Event, Aborted, To);
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
if (super.OnUpdate(DeltaTime, SimulationPrecision) == EXIT) return EXIT;
return CONTINUE;
}
}
class Expansion_Vehicles_Sitting_State_0 extends eAIState {
Expansion_Vehicles_FSM_0 fsm;
void Expansion_Vehicles_Sitting_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Vehicles_Sitting_State_0";
m_Name = "Sitting";
}
override void OnEntry(string Event, ExpansionState From) {
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
return EXIT;	
}
}
class Expansion_Vehicles_GoToVehicle_OpenVehicleDoor_Transition_0 extends eAITransition {
private Expansion_Vehicles_GoToVehicle_State_0 src;
private Expansion_Vehicles_OpenVehicleDoor_State_0 dst;
Expansion_Vehicles_FSM_0 fsm;
void Expansion_Vehicles_GoToVehicle_OpenVehicleDoor_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Vehicles_GoToVehicle_OpenVehicleDoor_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Vehicles_GoToVehicle_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Vehicles_OpenVehicleDoor_State_0"));
}
override int Guard() {
if (vector.Distance(unit.GetPosition(), src.position) > 0.5) return FAIL;
if (!dst.PerformTest(src.entity, src.seat)) return FAIL;	
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Vehicles_OpenVehicleDoor_GetInVehicle_Transition_0 extends eAITransition {
private Expansion_Vehicles_OpenVehicleDoor_State_0 src;
private Expansion_Vehicles_GetInVehicle_State_0 dst;
Expansion_Vehicles_FSM_0 fsm;
void Expansion_Vehicles_OpenVehicleDoor_GetInVehicle_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Vehicles_OpenVehicleDoor_GetInVehicle_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Vehicles_OpenVehicleDoor_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Vehicles_GetInVehicle_State_0"));
}
override int Guard() {
if (vector.Distance(unit.GetPosition(), src.position) > 0.5) return FAIL;	
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Vehicles_GetInVehicle_CloseVehicleDoor_Transition_0 extends eAITransition {
private Expansion_Vehicles_GetInVehicle_State_0 src;
private Expansion_Vehicles_CloseVehicleDoor_State_0 dst;
Expansion_Vehicles_FSM_0 fsm;
void Expansion_Vehicles_GetInVehicle_CloseVehicleDoor_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Vehicles_GetInVehicle_CloseVehicleDoor_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Vehicles_GetInVehicle_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Vehicles_CloseVehicleDoor_State_0"));
}
override int Guard() {
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Vehicles_CloseVehicleDoor_Sitting_Transition_0 extends eAITransition {
private Expansion_Vehicles_CloseVehicleDoor_State_0 src;
private Expansion_Vehicles_Sitting_State_0 dst;
Expansion_Vehicles_FSM_0 fsm;
void Expansion_Vehicles_CloseVehicleDoor_Sitting_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Vehicles_CloseVehicleDoor_Sitting_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Vehicles_CloseVehicleDoor_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Vehicles_Sitting_State_0"));
}
override int Guard() {
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Vehicles_Sitting_OpenVehicleDoor_Transition_0 extends eAITransition {
private Expansion_Vehicles_Sitting_State_0 src;
private Expansion_Vehicles_OpenVehicleDoor_State_0 dst;
Expansion_Vehicles_FSM_0 fsm;
void Expansion_Vehicles_Sitting_OpenVehicleDoor_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Vehicles_Sitting_OpenVehicleDoor_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Vehicles_Sitting_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Vehicles_OpenVehicleDoor_State_0"));
}
override int Guard() {
auto group = unit.GetGroup();	
if (!group) return SUCCESS;	
auto leader = group.GetLeader();	
if (!leader || leader == unit) return SUCCESS;	
if (group.GetFormationState() == eAIGroupFormationState.IN && leader.IsInTransport()) return FAIL;	
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Vehicles_OpenVehicleDoor_GetOutVehicle_Transition_0 extends eAITransition {
private Expansion_Vehicles_OpenVehicleDoor_State_0 src;
private Expansion_Vehicles_GetOutVehicle_State_0 dst;
Expansion_Vehicles_FSM_0 fsm;
void Expansion_Vehicles_OpenVehicleDoor_GetOutVehicle_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Vehicles_OpenVehicleDoor_GetOutVehicle_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Vehicles_OpenVehicleDoor_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Vehicles_GetOutVehicle_State_0"));
}
override int Guard() {
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Vehicles_GetOutVehicle_CloseVehicleDoor_Transition_0 extends eAITransition {
private Expansion_Vehicles_GetOutVehicle_State_0 src;
private Expansion_Vehicles_CloseVehicleDoor_State_0 dst;
Expansion_Vehicles_FSM_0 fsm;
void Expansion_Vehicles_GetOutVehicle_CloseVehicleDoor_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Vehicles_GetOutVehicle_CloseVehicleDoor_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Vehicles_GetOutVehicle_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Vehicles_CloseVehicleDoor_State_0"));
}
override int Guard() {
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Vehicles_CloseVehicleDoor__Transition_0 extends eAITransition {
private Expansion_Vehicles_CloseVehicleDoor_State_0 src;
private ExpansionState dst;
Expansion_Vehicles_FSM_0 fsm;
void Expansion_Vehicles_CloseVehicleDoor__Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Vehicles_CloseVehicleDoor__Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Vehicles_CloseVehicleDoor_State_0"));
Class.CastTo(dst, _fsm.GetState("ExpansionState"));
}
override int Guard() {
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Vehicles_FSM_0 extends eAIFSM {
EntityAI entity;
int seat;
void Expansion_Vehicles_FSM_0(ExpansionFSMOwnerType owner, ExpansionState parentState) {
m_Name = "Vehicles";
m_DefaultState = "Expansion_Vehicles_GoTo_State_0";
Setup();
}
void Setup() {
AddState(new Expansion_Vehicles_GoToVehicle_State_0(this));
AddState(new Expansion_Vehicles_GetInVehicle_State_0(this));
AddState(new Expansion_Vehicles_GetOutVehicle_State_0(this));
AddState(new Expansion_Vehicles_OpenVehicleDoor_State_0(this));
AddState(new Expansion_Vehicles_CloseVehicleDoor_State_0(this));
AddState(new Expansion_Vehicles_Sitting_State_0(this));
AddTransition(new Expansion_Vehicles_GoToVehicle_OpenVehicleDoor_Transition_0(this));
AddTransition(new Expansion_Vehicles_OpenVehicleDoor_GetInVehicle_Transition_0(this));
AddTransition(new Expansion_Vehicles_GetInVehicle_CloseVehicleDoor_Transition_0(this));
AddTransition(new Expansion_Vehicles_CloseVehicleDoor_Sitting_Transition_0(this));
AddTransition(new Expansion_Vehicles_Sitting_OpenVehicleDoor_Transition_0(this));
AddTransition(new Expansion_Vehicles_OpenVehicleDoor_GetOutVehicle_Transition_0(this));
AddTransition(new Expansion_Vehicles_GetOutVehicle_CloseVehicleDoor_Transition_0(this));
AddTransition(new Expansion_Vehicles_CloseVehicleDoor__Transition_0(this));
}
}
ExpansionFSM Create_Expansion_Vehicles_FSM_0(ExpansionFSMOwnerType owner, ExpansionState parentState) {
return new Expansion_Vehicles_FSM_0(owner, parentState);
}
class Expansion_Fighting_Positioning_State_0 extends eAIState {
Expansion_Fighting_FSM_0 fsm;
vector position;
float time;
float movementDirection;
void Expansion_Fighting_Positioning_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Fighting_Positioning_State_0";
m_Name = "Positioning";
}
override void OnEntry(string Event, ExpansionState From) {
time = 0;	
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
bool wantsLower = false;	
bool wantsRaise = false;	
if (GetGame().GetTime() - fsm.LastFireTime > fsm.TimeBetweenFiring)	
{	
wantsLower = true;	
}	
auto target = unit.GetTarget();	
if (target)	
{	
position = target.GetPosition(unit, false);	
auto aimPosition = position + target.GetAimOffset(unit);	
auto distanceSq = target.GetDistanceSq(unit, true);	
bool shouldBeMeleeing = false;	
auto hands = unit.GetHumanInventory().GetEntityInHands();	
if (target.GetEntity().IsInherited(ItemBase))	
{	
wantsLower = true;	
}	
else if (!hands)	
{	
shouldBeMeleeing = true;	
}	
else if (hands.IsWeapon())	
{	
if (distanceSq <= 2.25)	
{	
shouldBeMeleeing = true;	
}	
}	
else if (hands.IsMeleeWeapon())	
{	
shouldBeMeleeing = true;	
}	
if (shouldBeMeleeing)	
{	
if (distanceSq <= 3.24)	
{	
wantsRaise = true;	
}	
else	
{	
wantsLower = true;	
}	
}	
if (distanceSq <= 1.0)	
{	
time += DeltaTime;	
//unit.OverrideStance(DayZPlayerConstants.STANCEIDX_RAISEDERECT);	
if (!movementDirection || time > Math.RandomIntInclusive(1, 3))	
{	
if (Math.RandomIntInclusive(0, 1))	
movementDirection = Math.RandomFloat(135, 180);	
else	
movementDirection = Math.RandomFloat(-135, -180);	
}	
unit.OverrideMovementDirection(true, movementDirection);	
unit.OverrideMovementSpeed(true, Math.RandomIntInclusive(1, 2));	
}	
else	
{	
//unit.OverrideStance(0);	
unit.OverrideMovementDirection(false, 0);	
unit.OverrideMovementSpeed(false, 0);	
time = 0;	
movementDirection= 0;	
}	
unit.LookAtPosition(aimPosition);	
unit.AimAtPosition(aimPosition);	
unit.OverrideTargetPosition(position);	
if (hands && (hands.IsWeapon() || distanceSq <= 100.0))	
{	
if (hands.HasEnergyManager() && !hands.GetCompEM().IsWorking() && hands.GetCompEM().CanSwitchOn())	
{	
hands.GetCompEM().SwitchOn();	
}	
}	
}	
else	
{	
unit.OverrideMovementDirection(false, 0);	
unit.OverrideMovementSpeed(false, 0);	
}	
if (wantsRaise && unit.CanRaiseWeapon())	
{	
unit.RaiseWeapon(true);	
}	
else if (wantsLower || !unit.CanRaiseWeapon())	
{	
unit.RaiseWeapon(false);	
}	
return EXIT;	
}
}
class Expansion_Fighting_FireWeapon_State_0 extends eAIState {
Expansion_Fighting_FSM_0 fsm;
float time;
eAITarget target;
void Expansion_Fighting_FireWeapon_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Fighting_FireWeapon_State_0";
m_Name = "FireWeapon";
}
override void OnEntry(string Event, ExpansionState From) {
unit.RaiseWeapon(true);	
time = 0;	
fsm.LastFireTime = GetGame().GetTime();	
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
if (!target)	
return EXIT;	
auto lowPosition = target.GetPosition(unit, false);	
auto aimPosition = lowPosition + target.GetAimOffset(unit);	
time += DeltaTime;	
unit.OverrideTargetPosition(lowPosition);	
unit.LookAtPosition(aimPosition);	
unit.AimAtPosition(aimPosition);	
if (!unit.IsRaised() || !unit.IsWeaponRaiseCompleted())	
{	
unit.RaiseWeapon(true);	
if (time >= 0.5)	
{	
return EXIT;	
}	
// waiting for the weapon to be raised	
return CONTINUE;	
}	
unit.TryFireWeapon();	
return EXIT;	
}
}
class Expansion_Fighting_Melee_State_0 extends eAIState {
Expansion_Fighting_FSM_0 fsm;
float time;
eAITarget target;
float movementDirection;
void Expansion_Fighting_Melee_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Fighting_Melee_State_0";
m_Name = "Melee";
}
override void OnEntry(string Event, ExpansionState From) {
time = 0;	
fsm.LastFireTime = GetGame().GetTime();	
unit.Expansion_GetUp();	
//! FIXME: Pistols fuck up the hand animation state.	
//! Ugly workaround: Put away when entering melee.	
auto hands = unit.GetItemInHands();	
if (hands && hands.IsKindOf("Pistol_Base"))	
{	
unit.eAI_TakeItemToInventory(hands);	
}	
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
if (!target)	
return EXIT;	
auto aimOffset = target.GetAimOffset(unit);	
auto lowPosition = target.GetPosition(unit, false);	
auto aimPosition = lowPosition + aimOffset;	
time += DeltaTime;	
unit.OverrideTargetPosition(lowPosition);	
unit.LookAtPosition(aimPosition);	
unit.AimAtPosition(aimPosition);	
float distanceSq = target.GetDistanceSq(unit, true);	
if (distanceSq > 2.25)	
{	
if (time >= 0.5)	
{	
time = 0;	
return EXIT;	
}	
return CONTINUE;	
}	
auto direction = vector.Direction(unit.GetPosition(), lowPosition).Normalized();	
if (vector.Dot(unit.GetDirection(), direction) < 0.75)	
{	
if (time >= Math.RandomIntInclusive(1, 3))	
{	
//unit.OverrideStance(0);	
unit.OverrideMovementDirection(false, 0);	
unit.OverrideMovementSpeed(false, 0);	
time = 0;	
movementDirection = 0;	
return EXIT;	
}	
//unit.OverrideStance(DayZPlayerConstants.STANCEIDX_RAISEDERECT);	
if (!movementDirection || time > Math.RandomIntInclusive(1, 3))	
{	
if (Math.RandomIntInclusive(0, 1))	
movementDirection = Math.RandomFloat(135, 180);	
else	
movementDirection = Math.RandomFloat(-135, -180);	
}	
unit.OverrideMovementDirection(true, movementDirection);	
unit.OverrideMovementSpeed(true, Math.RandomIntInclusive(1, 2));	
return CONTINUE;	
}	
if (unit.IsInMelee() && time < 0.3)	
{	
return CONTINUE;	
}	
unit.Notify_Melee();	
time = 0;	
movementDirection = 0;	
return EXIT;	
}
}
class Expansion_Fighting__Melee_Transition_0 extends eAITransition {
private ExpansionState src;
private Expansion_Fighting_Melee_State_0 dst;
Expansion_Fighting_FSM_0 fsm;
void Expansion_Fighting__Melee_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Fighting__Melee_Transition_0";
Class.CastTo(src, _fsm.GetState("ExpansionState"));
Class.CastTo(dst, _fsm.GetState("Expansion_Fighting_Melee_State_0"));
}
override int Guard() {
// we are targetting an entity?	
dst.target = unit.GetTarget();	
if (!dst.target || !dst.target.IsMeleeViable(unit)) return FAIL;	
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Fighting__FireWeapon_Transition_0 extends eAITransition {
private ExpansionState src;
private Expansion_Fighting_FireWeapon_State_0 dst;
Expansion_Fighting_FSM_0 fsm;
void Expansion_Fighting__FireWeapon_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Fighting__FireWeapon_Transition_0";
Class.CastTo(src, _fsm.GetState("ExpansionState"));
Class.CastTo(dst, _fsm.GetState("Expansion_Fighting_FireWeapon_State_0"));
}
override int Guard() {
// we are aiming at something?	
dst.target = unit.GetTarget();	
if (!dst.target) return FAIL;	
if (unit.IsInMelee()) return FAIL;	
// we are holding a weapon	
Weapon_Base weapon;	
if (!Class.CastTo(weapon, unit.GetItemInHands())) return FAIL;	
// CanRaiseWeapon will return false if there is no line of sight	
if (!unit.CanRaiseWeapon()) return FAIL;	
if (!weapon.Expansion_IsChambered()) return FAIL;	
if (unit.GetWeaponManager().CanUnjam(weapon)) return FAIL;	
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Fighting__Positioning_Transition_0 extends eAITransition {
private ExpansionState src;
private Expansion_Fighting_Positioning_State_0 dst;
Expansion_Fighting_FSM_0 fsm;
void Expansion_Fighting__Positioning_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Fighting__Positioning_Transition_0";
Class.CastTo(src, _fsm.GetState("ExpansionState"));
Class.CastTo(dst, _fsm.GetState("Expansion_Fighting_Positioning_State_0"));
}
override int Guard() {
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Fighting_FSM_0 extends eAIFSM {
int LastFireTime;
int TimeBetweenFiring = 5000;
void Expansion_Fighting_FSM_0(ExpansionFSMOwnerType owner, ExpansionState parentState) {
m_Name = "Fighting";
m_DefaultState = "Expansion_Fighting_Positioning_State_0";
Setup();
}
void Setup() {
AddState(new Expansion_Fighting_Positioning_State_0(this));
AddState(new Expansion_Fighting_FireWeapon_State_0(this));
AddState(new Expansion_Fighting_Melee_State_0(this));
AddTransition(new Expansion_Fighting__Melee_Transition_0(this));
AddTransition(new Expansion_Fighting__FireWeapon_Transition_0(this));
AddTransition(new Expansion_Fighting__Positioning_Transition_0(this));
}
}
ExpansionFSM Create_Expansion_Fighting_FSM_0(ExpansionFSMOwnerType owner, ExpansionState parentState) {
return new Expansion_Fighting_FSM_0(owner, parentState);
}
class Expansion_Reloading_Start_State_0 extends eAIState {
Expansion_Reloading_FSM_0 fsm;
void Expansion_Reloading_Start_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Reloading_Start_State_0";
m_Name = "Start";
}
override void OnEntry(string Event, ExpansionState From) {
fsm.last_attempt_time = GetGame().GetTime();	
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
return EXIT;	
}
}
class Expansion_Reloading_Reloading_State_0 extends eAIState {
Expansion_Reloading_FSM_0 fsm;
Magazine magazine;
float time;
void Expansion_Reloading_Reloading_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Reloading_Reloading_State_0";
m_Name = "Reloading";
}
override void OnEntry(string Event, ExpansionState From) {
time = 0;	
unit.RaiseWeapon(true);	
unit.ReloadWeaponAI(fsm.weapon, magazine);	
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
unit.OverrideMovementDirection(false, 0);	
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
if (!unit.GetWeaponManager() || unit.IsUnconscious()) return EXIT;	
if (unit.GetWeaponManager().IsRunning())	
{	
time += DeltaTime;	
if (time > 12)  //! Looks like something went terribly wrong	
{	
EXTrace.Print(true, unit, "Weapon_Reloading - Reloading - timeout");	
unit.eAI_Unbug("reload");	
return EXIT;	
}	
auto target = unit.GetTarget();	
if (target && target.GetDistanceSq(unit, true) <= 2.25)	
{	
unit.OverrideMovementDirection(true, -180);	
}	
return CONTINUE;	
}	
if (!fsm.weapon) return EXIT;	
int mi = fsm.weapon.GetCurrentMuzzle();	
if (fsm.weapon.IsChamberEmpty(mi))	
{	
fsm.failed_attempts++;	
EXTrace.Print(true, unit, "Weapon_Reloading - Reloading - failed (" + fsm.failed_attempts + ")");	
fsm.weapon.ValidateAndRepair();	
}	
else	
{	
fsm.failed_attempts = 0;	
}	
return EXIT;	
}
}
class Expansion_Reloading_Reloading_Fail_State_0 extends eAIState {
Expansion_Reloading_FSM_0 fsm;
float time;
void Expansion_Reloading_Reloading_Fail_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Reloading_Reloading_Fail_State_0";
m_Name = "Reloading_Fail";
}
override void OnEntry(string Event, ExpansionState From) {
unit.RaiseWeapon(false);	
time = 0;	
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
time += DeltaTime;	
// waiting for the weapon to be lowered	
if (fsm.weapon && time < 0.5)	
return CONTINUE;	
return EXIT;	
}
}
class Expansion_Reloading_Removing_State_0 extends eAIState {
Expansion_Reloading_FSM_0 fsm;
void Expansion_Reloading_Removing_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Reloading_Removing_State_0";
m_Name = "Removing";
}
override void OnEntry(string Event, ExpansionState From) {
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
if (!fsm.weapon || unit.GetItemInHands() != fsm.weapon)	
return EXIT;  // remove complete	
if (!unit.eAI_TakeItemToInventory(fsm.weapon))	
unit.eAI_DropItem(fsm.weapon);	
return CONTINUE;	
}
}
class Expansion_Reloading_Start_Reloading_Transition_0 extends eAITransition {
private Expansion_Reloading_Start_State_0 src;
private Expansion_Reloading_Reloading_State_0 dst;
Expansion_Reloading_FSM_0 fsm;
void Expansion_Reloading_Start_Reloading_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Reloading_Start_Reloading_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Reloading_Start_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Reloading_Reloading_State_0"));
}
override int Guard() {
if (!fsm.weapon || fsm.weapon.IsDamageDestroyed())	
return FAIL;	
if (!unit.eAI_HasAmmoForFirearm(fsm.weapon, dst.magazine)) return FAIL;	
if (!dst.magazine)	
EXTrace.Start0(EXTrace.AI, this, "Reloading " + fsm.weapon + " from internal mag");	
else	
EXTrace.Start0(EXTrace.AI, this, "Reloading " + fsm.weapon + " from mag " + dst.magazine);	
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Reloading_Start_Reloading_Fail_Transition_0 extends eAITransition {
private Expansion_Reloading_Start_State_0 src;
private Expansion_Reloading_Reloading_Fail_State_0 dst;
Expansion_Reloading_FSM_0 fsm;
void Expansion_Reloading_Start_Reloading_Fail_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Reloading_Start_Reloading_Fail_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Reloading_Start_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Reloading_Reloading_Fail_State_0"));
}
override int Guard() {
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Reloading_Reloading_Fail_Removing_Transition_0 extends eAITransition {
private Expansion_Reloading_Reloading_Fail_State_0 src;
private Expansion_Reloading_Removing_State_0 dst;
Expansion_Reloading_FSM_0 fsm;
void Expansion_Reloading_Reloading_Fail_Removing_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Reloading_Reloading_Fail_Removing_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Reloading_Reloading_Fail_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Reloading_Removing_State_0"));
}
override int Guard() {
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Reloading_Reloading__Transition_0 extends eAITransition {
private Expansion_Reloading_Reloading_State_0 src;
private ExpansionState dst;
Expansion_Reloading_FSM_0 fsm;
void Expansion_Reloading_Reloading__Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Reloading_Reloading__Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Reloading_Reloading_State_0"));
Class.CastTo(dst, _fsm.GetState("ExpansionState"));
}
override int Guard() {
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Reloading_Removing__Transition_0 extends eAITransition {
private Expansion_Reloading_Removing_State_0 src;
private ExpansionState dst;
Expansion_Reloading_FSM_0 fsm;
void Expansion_Reloading_Removing__Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Reloading_Removing__Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Reloading_Removing_State_0"));
Class.CastTo(dst, _fsm.GetState("ExpansionState"));
}
override int Guard() {
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Reloading_FSM_0 extends eAIFSM {
Weapon_Base weapon;
int last_attempt_time;
int failed_attempts;
void Expansion_Reloading_FSM_0(ExpansionFSMOwnerType owner, ExpansionState parentState) {
m_Name = "Reloading";
m_DefaultState = "Expansion_Reloading_Start_State_0";
Setup();
}
void Setup() {
AddState(new Expansion_Reloading_Start_State_0(this));
AddState(new Expansion_Reloading_Reloading_State_0(this));
AddState(new Expansion_Reloading_Reloading_Fail_State_0(this));
AddState(new Expansion_Reloading_Removing_State_0(this));
AddTransition(new Expansion_Reloading_Start_Reloading_Transition_0(this));
AddTransition(new Expansion_Reloading_Start_Reloading_Fail_Transition_0(this));
AddTransition(new Expansion_Reloading_Reloading_Fail_Removing_Transition_0(this));
AddTransition(new Expansion_Reloading_Reloading__Transition_0(this));
AddTransition(new Expansion_Reloading_Removing__Transition_0(this));
}
}
ExpansionFSM Create_Expansion_Reloading_FSM_0(ExpansionFSMOwnerType owner, ExpansionState parentState) {
return new Expansion_Reloading_FSM_0(owner, parentState);
}
class Expansion_Master_Idle_State_0 extends eAIState {
Expansion_Master_FSM_0 fsm;
void Expansion_Master_Idle_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_Idle_State_0";
m_Name = "Idle";
}
override void OnEntry(string Event, ExpansionState From) {
if (!unit.GetTarget())	
{	
if (unit.GetLookDirectionRecalculate())	
unit.LookAtDirection("0 0 1");	
if (unit.GetAimDirectionRecalculate())	
unit.AimAtDirection("0 0 1");	
}	
auto hands = unit.GetItemInHands();	
if (hands && hands.HasEnergyManager() && hands.GetCompEM().IsWorking() && hands.GetCompEM().CanSwitchOff())	
{	
hands.GetCompEM().SwitchOff();	
}	
unit.OverrideMovementDirection(false, 0);	
unit.OverrideMovementSpeed(true, 0);	
unit.Expansion_GetUp();	
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
return EXIT;	
}
}
class Expansion_Master_Unconscious_State_0 extends eAIState {
Expansion_Master_FSM_0 fsm;
float time;
void Expansion_Master_Unconscious_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_Unconscious_State_0";
m_Name = "Unconscious";
}
override void OnEntry(string Event, ExpansionState From) {
time = 0;	
unit.OverrideTargetPosition(unit.GetPosition());	
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
if (time > 3)	
{	
return EXIT;	
}	
if (!unit.IsUnconscious())	
{	
time += DeltaTime;  //! Allow time to stand up so we don't instantly start firing	
}	
return CONTINUE;	
}
}
class Expansion_Master_Trading_State_0 extends eAIState {
Expansion_Master_FSM_0 fsm;
void Expansion_Master_Trading_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_Trading_State_0";
m_Name = "Trading";
}
override void OnEntry(string Event, ExpansionState From) {
unit.OverrideTargetPosition(unit.GetPosition());	
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
if (unit.IsTrading())	
{	
return CONTINUE;	
}	
return EXIT;	
}
}
class Expansion_Master_FollowFormation_State_0 extends eAIState {
Expansion_Master_FSM_0 fsm;
eAIGroup group;
int speedLimit;
void Expansion_Master_FollowFormation_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_FollowFormation_State_0";
m_Name = "FollowFormation";
}
override void OnEntry(string Event, ExpansionState From) {
unit.Expansion_GetUp();	
speedLimit = unit.GetMovementSpeedLimit();	
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
unit.SetMovementSpeedLimit(speedLimit);  //! Restore speed limit	
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
unit.OverrideTargetPosition(group.GetFormationPosition(unit));	
unit.OverrideMovementDirection(false, 0);	
unit.OverrideMovementSpeed(false, 0);	
unit.SetMovementSpeedLimit(3);  //! Make sure AI can reach formation positions when following leader by overriding speed limit 	
return EXIT;	
}
}
class Expansion_Master_TraversingWaypoints_State_0 extends eAIState {
Expansion_Master_FSM_0 fsm;
ref TVectorArray path;
eAIWaypointBehavior behaviour;
bool backtracking;
int index;
float threshold = 1.0;
float previousDistance;
vector previousWayPoint;
void Expansion_Master_TraversingWaypoints_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_TraversingWaypoints_State_0";
m_Name = "TraversingWaypoints";
}
override void OnEntry(string Event, ExpansionState From) {
path = unit.GetGroup().GetWaypoints();	
if (path.Count() == 0)	
{	
path = { unit.GetPosition() };	
}	
behaviour = unit.GetGroup().GetWaypointBehaviour();	
unit.Expansion_GetUp();	
if (previousWayPoint == vector.Zero && path.Count() > 1)	
previousWayPoint = path[0] - vector.Direction(path[0], path[1]).Normalized();	
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
index = unit.GetGroup().m_CurrentWaypointIndex;	
backtracking = unit.GetGroup().m_BackTracking;	
float distance = vector.DistanceSq(unit.GetPosition(), path[index]);	
if (distance < threshold)	
{	
previousWayPoint = path[index];	
if (backtracking) index--;	
else index++;	
threshold = 1.0;	
}	
else if (Math.AbsFloat(distance - previousDistance) < 0.01)	
{	
//! We seem to not be getting closer to the waypoint, possibly the path is blocked.	
//! Increase threshold until we are within distance.	
threshold += 0.01;	
}	
previousDistance = distance;	
if (index < 0) 	
{	
if (behaviour == eAIWaypointBehavior.ALTERNATE)	
{	
backtracking = false;	
index = 1;	
}	
else	
{	
index = path.Count() - 1;	
}	
}	
else if (index == path.Count())	
{	
if (behaviour == eAIWaypointBehavior.ALTERNATE)	
{	
backtracking = true;	
index = path.Count() - 2;	
} 	
else if (behaviour == eAIWaypointBehavior.LOOP)	
{	
index = 0;	
}	
}	
index = Math.Clamp(index, 0, path.Count() - 1);	
bool isFinal;	
if (behaviour != eAIWaypointBehavior.LOOP)	
isFinal = index == 0 || index == path.Count() - 1;	
unit.OverrideTargetPosition(path[index], isFinal);	
unit.OverrideMovementDirection(false, 0);	
unit.OverrideMovementSpeed(false, 0);	
vector direction;	
if (path.Count() > 1)	
direction = vector.Direction(previousWayPoint, path[index]).Normalized();	
else	
direction = unit.GetDirection();	
unit.Expansion_DebugObject_Deferred(index + 20, path[index] - "0 1.5 0", "ExpansionDebugNoticeMe_Red", direction);	
unit.Expansion_DebugObject_Deferred(path.Count() + 20, path[index], "ExpansionDebugNoticeMe", unit.GetDirection());	
unit.GetGroup().m_CurrentWaypointIndex = index;	
unit.GetGroup().m_BackTracking = backtracking;	
return EXIT;	
}
}
class Expansion_Master_Vehicles_State_0 extends eAIState {
Expansion_Vehicles_FSM_0 sub_fsm;
Expansion_Master_FSM_0 fsm;
EntityAI entity;
int seat;
void Expansion_Master_Vehicles_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_Vehicles_State_0";
m_Name = "Vehicles";
m_SubFSM = new Expansion_Vehicles_FSM_0(_fsm.GetOwner(), this);
Class.CastTo(sub_fsm, m_SubFSM);
}
override void OnEntry(string Event, ExpansionState From) {
if (Event != "") m_SubFSM.Start(Event);
else m_SubFSM.StartDefault();
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
if (Aborted) m_SubFSM.Abort(Event);
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
if (m_SubFSM.Update(DeltaTime, SimulationPrecision) == EXIT) return EXIT;
auto group = unit.GetGroup();	
if (!group) return EXIT;	
auto leader = group.GetLeader();	
if (!leader) return EXIT;
if (leader == unit)	
{	
if (!entity) return EXIT;
//! TODO: Allow for exit vehicle since this AI is the leader	
return CONTINUE;	
}	
//! MAYBE BUG? Might deadlock the ai if there are no free seats for the vehicle in the group	
if (group.GetFormationState() == eAIGroupFormationState.IN && leader.IsInTransport()) 	
{	
Transport transport;	
if (!Class.CastTo(transport, leader.GetParent())) return EXIT;
for (int i = 0; i < transport.CrewSize(); i++)	
{	
if (transport.CrewMember(i) == null)	
{	
seat = i;	
entity = transport;
return CONTINUE;	
}	
}	
}	
return EXIT;	
}
}
class Expansion_Master_Fighting_State_0 extends eAIState {
Expansion_Fighting_FSM_0 sub_fsm;
Expansion_Master_FSM_0 fsm;
void Expansion_Master_Fighting_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_Fighting_State_0";
m_Name = "Fighting";
m_SubFSM = new Expansion_Fighting_FSM_0(_fsm.GetOwner(), this);
Class.CastTo(sub_fsm, m_SubFSM);
}
override void OnEntry(string Event, ExpansionState From) {
if (Event != "") m_SubFSM.Start(Event);
else m_SubFSM.StartDefault();
if (unit.GetEmoteManager().IsEmotePlaying())	
unit.GetEmoteManager().ServerRequestEmoteCancel();	
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
if (Aborted) m_SubFSM.Abort(Event);
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
if (m_SubFSM.Update(DeltaTime, SimulationPrecision) == EXIT) return EXIT;
return EXIT;	
}
}
class Expansion_Master_Weapon_Reloading_State_0 extends eAIState {
Expansion_Reloading_FSM_0 sub_fsm;
Expansion_Master_FSM_0 fsm;
void Expansion_Master_Weapon_Reloading_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_Weapon_Reloading_State_0";
m_Name = "Reloading";
m_SubFSM = new Expansion_Reloading_FSM_0(_fsm.GetOwner(), this);
Class.CastTo(sub_fsm, m_SubFSM);
}
override void OnEntry(string Event, ExpansionState From) {
if (Event != "") m_SubFSM.Start(Event);
else m_SubFSM.StartDefault();
if (unit.GetEmoteManager().IsEmotePlaying())	
unit.GetEmoteManager().ServerRequestEmoteCancel();	
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
if (Aborted) m_SubFSM.Abort(Event);
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
if (m_SubFSM.Update(DeltaTime, SimulationPrecision) == EXIT) return EXIT;
return CONTINUE;
}
}
class Expansion_Master_Weapon_Unjamming_State_0 extends eAIState {
Expansion_Master_FSM_0 fsm;
Weapon_Base weapon;
float time;
int failed_attempts;
void Expansion_Master_Weapon_Unjamming_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_Weapon_Unjamming_State_0";
m_Name = "Weapon_Unjamming";
}
override void OnEntry(string Event, ExpansionState From) {
time = 0;	
unit.RaiseWeapon(true);	
unit.StartActionObject(eAIActionWeaponUnjam, null);	
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
unit.RaiseWeapon(false);	
unit.OverrideMovementDirection(false, 0);	
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
if (!unit.GetWeaponManager() || unit.IsUnconscious()) return EXIT;	
if (unit.GetWeaponManager().IsRunning())	
{	
time += DeltaTime;	
if (time > 10)  //! Looks like something went terribly wrong	
{	
EXTrace.Print(true, unit, "Weapon_Unjamming - timeout");	
unit.eAI_Unbug("unjam");	
return EXIT;	
}	
auto target = unit.GetTarget();	
if (target && target.GetDistanceSq(unit, true) <= 2.25)	
{	
unit.OverrideMovementDirection(true, -180);	
}	
return CONTINUE;	
}	
if (unit.GetWeaponManager().CanUnjam(weapon))	
{	
failed_attempts++;	
EXTrace.Print(true, unit, "Weapon_Unjamming - failed (" + failed_attempts + ")");	
weapon.ValidateAndRepair();	
if (failed_attempts > 5)	
{	
unit.eAI_DropItem(weapon);	
}	
}	
else	
{	
failed_attempts = 0;	
}	
return EXIT;	
}
}
class Expansion_Master_TakeItemToHands_State_0 extends eAIState {
Expansion_Master_FSM_0 fsm;
ItemBase item;
float time;
void Expansion_Master_TakeItemToHands_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_TakeItemToHands_State_0";
m_Name = "TakeItemToHands";
}
override void OnEntry(string Event, ExpansionState From) {
EXTrace.Print(EXTrace.AI, unit, "TakeItemToHands " + item.ToString());	
time = 0;	
unit.eAI_TakeItemToHands(item);	
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
if (time < 0.5)	
{	
time += DeltaTime;	
return CONTINUE;	
}	
return EXIT;	
}
}
class Expansion_Master_Bandaging_Self_State_0 extends eAIState {
Expansion_Master_FSM_0 fsm;
int last_bandage_attempt_time;
ItemBase bandage;
float timeout;
float time;
void Expansion_Master_Bandaging_Self_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_Bandaging_Self_State_0";
m_Name = "Bandaging_Self";
}
override void OnEntry(string Event, ExpansionState From) {
last_bandage_attempt_time = GetGame().GetTime();	
time = 0;	
float effectivity = bandage.GetBandagingEffectivity();	
if (effectivity > 0)	
timeout = UATimeSpent.BANDAGE / effectivity + 8.0;	
else	
timeout = 16.0;	
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
unit.Expansion_GetUp(true);	
if (bandage)	
{	
if (bandage.GetHealth() <= 0.0 || !unit.eAI_TakeItemToInventory(bandage))	
{	
unit.eAI_DropItem(bandage);	
}	
}	
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
if (unit.IsUnconscious()) return EXIT;	
if (unit.GetActionManager().GetRunningAction())	
{	
time += DeltaTime;	
if (time > timeout)  //! Looks like something went terribly wrong	
{	
EXTrace.Print(true, unit, "Bandaging_Self - timeout");	
unit.eAI_Unbug("bandage");	
time = 0;	
return EXIT;	
}	
return CONTINUE;	
}	
else	
{	
if (bandage)	
{	
if (unit.GetBleedingSourceCount() && bandage.GetHealth() > 0.0)	
{	
last_bandage_attempt_time = GetGame().GetTime();	
time = 0;	
unit.StartActionObject(ActionBandageSelf, null);	
return CONTINUE;	
}	
}	
}	
return EXIT;	
}
}
class Expansion_Master_PlayEmote_State_0 extends eAIState {
Expansion_Master_FSM_0 fsm;
void Expansion_Master_PlayEmote_State_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_PlayEmote_State_0";
m_Name = "PlayEmote";
}
override void OnEntry(string Event, ExpansionState From) {
unit.Expansion_PlayEmote();	
}
override void OnExit(string Event, bool Aborted, ExpansionState To) {
}
override int OnUpdate(float DeltaTime, int SimulationPrecision) {
return EXIT;	
}
}
class Expansion_Master__Unconscious_Transition_0 extends eAITransition {
private ExpansionState src;
private Expansion_Master_Unconscious_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master__Unconscious_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master__Unconscious_Transition_0";
Class.CastTo(src, _fsm.GetState("ExpansionState"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_Unconscious_State_0"));
}
override int Guard() {
if (!(unit.IsUnconscious())) return FAIL;	
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master_Unconscious_Idle_Transition_0 extends eAITransition {
private Expansion_Master_Unconscious_State_0 src;
private Expansion_Master_Idle_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master_Unconscious_Idle_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_Unconscious_Idle_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Master_Unconscious_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_Idle_State_0"));
}
override int Guard() {
if (unit.IsUnconscious()) return FAIL;	
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master__Trading_Transition_0 extends eAITransition {
private ExpansionState src;
private Expansion_Master_Trading_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master__Trading_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master__Trading_Transition_0";
Class.CastTo(src, _fsm.GetState("ExpansionState"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_Trading_State_0"));
}
override int Guard() {
if (!(unit.IsTrading())) return FAIL;	
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master_Trading_Idle_Transition_0 extends eAITransition {
private Expansion_Master_Trading_State_0 src;
private Expansion_Master_Idle_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master_Trading_Idle_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_Trading_Idle_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Master_Trading_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_Idle_State_0"));
}
override int Guard() {
if (unit.IsTrading()) return FAIL;	
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master__Bandaging_Self_Transition_0 extends eAITransition {
private ExpansionState src;
private Expansion_Master_Bandaging_Self_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master__Bandaging_Self_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master__Bandaging_Self_Transition_0";
Class.CastTo(src, _fsm.GetState("ExpansionState"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_Bandaging_Self_State_0"));
}
override int Guard() {
if (unit.IsInMelee()) return FAIL;	
if (!unit.GetBleedingSourceCount()) return FAIL;	
if (GetGame().GetTime() - dst.last_bandage_attempt_time < 4000) return FAIL;	
auto hands = unit.GetItemInHands();	
if (!hands) return FAIL;	
if (!(hands.IsInherited(BandageDressing) || hands.IsInherited(Rag)) || hands.GetHealth() <= 0.0) return FAIL;	
dst.bandage = hands;	
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master_Bandaging_Self_Idle_Transition_0 extends eAITransition {
private Expansion_Master_Bandaging_Self_State_0 src;
private Expansion_Master_Idle_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master_Bandaging_Self_Idle_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_Bandaging_Self_Idle_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Master_Bandaging_Self_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_Idle_State_0"));
}
override int Guard() {
if (unit.GetActionManager().GetRunningAction()) return FAIL;	
if (GetGame().GetTime() - src.last_bandage_attempt_time < 4000) return FAIL;	
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master_Idle_FollowFormation_Transition_0 extends eAITransition {
private Expansion_Master_Idle_State_0 src;
private Expansion_Master_FollowFormation_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master_Idle_FollowFormation_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_Idle_FollowFormation_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Master_Idle_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_FollowFormation_State_0"));
}
override int Guard() {
if (unit.GetThreatToSelf() > 0.4) return FAIL;	
dst.group = unit.GetGroup();	
if (!dst.group) return FAIL;	
if (dst.group.GetFormationState() != eAIGroupFormationState.IN) return FAIL;	
auto leader = dst.group.GetLeader();	
if (!leader || leader == unit) return FAIL;	
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master_Idle_TraversingWaypoints_Transition_0 extends eAITransition {
private Expansion_Master_Idle_State_0 src;
private Expansion_Master_TraversingWaypoints_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master_Idle_TraversingWaypoints_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_Idle_TraversingWaypoints_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Master_Idle_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_TraversingWaypoints_State_0"));
}
override int Guard() {
if (unit.GetThreatToSelf() > 0.4) return FAIL;	
auto group = unit.GetGroup();	
if (!group) return FAIL;	
// we are the leader so we traverse the waypoints	
auto leader = group.GetLeader();	
if (leader && leader != unit) return FAIL;	
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master_TraversingWaypoints_Idle_Transition_0 extends eAITransition {
private Expansion_Master_TraversingWaypoints_State_0 src;
private Expansion_Master_Idle_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master_TraversingWaypoints_Idle_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_TraversingWaypoints_Idle_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Master_TraversingWaypoints_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_Idle_State_0"));
}
override int Guard() {
if (unit.GetThreatToSelf() > 0.4) return SUCCESS;	
return FAIL;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master_FollowFormation_Idle_Transition_0 extends eAITransition {
private Expansion_Master_FollowFormation_State_0 src;
private Expansion_Master_Idle_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master_FollowFormation_Idle_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_FollowFormation_Idle_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Master_FollowFormation_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_Idle_State_0"));
}
override int Guard() {
auto group = unit.GetGroup();	
if (!group || group.GetLeader() == unit || group.GetFormationState() != eAIGroupFormationState.IN) return SUCCESS;	
if (unit.GetThreatToSelf() > 0.4) return SUCCESS;	
return FAIL;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master__Weapon_Reloading_Transition_0 extends eAITransition {
private ExpansionState src;
private Expansion_Master_Weapon_Reloading_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master__Weapon_Reloading_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master__Weapon_Reloading_Transition_0";
Class.CastTo(src, _fsm.GetState("ExpansionState"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_Weapon_Reloading_State_0"));
}
override int Guard() {
if (GetGame().GetTime() - dst.sub_fsm.last_attempt_time < 1000) return FAIL;	
if (unit.IsInMelee()) return FAIL;	
if (!Class.CastTo(dst.sub_fsm.weapon, unit.GetItemInHands())) return FAIL;	
//! Allow sub-FSM to handle destroyed weapon so it gets dropped	
if (dst.sub_fsm.weapon.IsDamageDestroyed()) return SUCCESS;	
if (dst.sub_fsm.weapon.Expansion_IsChambered()) return FAIL;	
if (unit.GetWeaponManager().CanUnjam(dst.sub_fsm.weapon)) return FAIL;	
// don't move to the state if the action manager is operating	
if (!unit.GetActionManager() || unit.GetActionManager().GetRunningAction()) return FAIL;	
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master__TakeItemToHands_Transition_0 extends eAITransition {
private ExpansionState src;
private Expansion_Master_TakeItemToHands_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master__TakeItemToHands_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master__TakeItemToHands_Transition_0";
Class.CastTo(src, _fsm.GetState("ExpansionState"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_TakeItemToHands_State_0"));
}
override int Guard() {
if (unit.IsInMelee()) return FAIL;	
//! Taking items to hands while raised breaks hands! Wait until lowered	
if (unit.IsRaised()) return FAIL;	
ItemBase hands = unit.GetItemInHands();	
//! First check if we want to switch to bandage	
if (unit.GetBleedingSourceCount() && unit.GetThreatToSelf(true) < 0.4)	
{	
if (!hands || !(hands.IsInherited(BandageDressing) || hands.IsInherited(Rag)) || hands.GetHealth() <= 0.0)	
{	
//! Item in hand is either not bandage/rag or is ruined	
dst.item = unit.GetBandageToUse();	
if (dst.item)	
{	
//! If ruined, drop, else put in inventory (shoulder slot or cargo)	
if (hands && (hands.GetHealth() <= 0.0 || !unit.eAI_TakeItemToInventory(hands)))	
unit.eAI_DropItem(hands);	
return SUCCESS;	
}	
}	
}	
if (hands)	
return FAIL;	
dst.item = unit.GetWeaponToUse(true);	
if (dst.item)	
return SUCCESS;	
eAITarget target = unit.GetTarget();	
if (target && target.GetEntity().IsInherited(ItemBase) && !target.GetEntity().GetHierarchyRootPlayer() && !target.GetEntity().IsSetForDeletion())	
{	
if (target.GetDistanceSq(unit, true) < 2.25 && target.GetThreat(unit) > 0.1)	
{	
dst.item = ItemBase.Cast(target.GetEntity());	
}	
}	
if (dst.item)	
return SUCCESS;	
dst.item = unit.GetMeleeWeaponToUse();	
if (dst.item)	
return SUCCESS;	
return FAIL;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master_TakeItemToHands_Idle_Transition_0 extends eAITransition {
private Expansion_Master_TakeItemToHands_State_0 src;
private Expansion_Master_Idle_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master_TakeItemToHands_Idle_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_TakeItemToHands_Idle_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Master_TakeItemToHands_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_Idle_State_0"));
}
override int Guard() {
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master__Weapon_Unjamming_Transition_0 extends eAITransition {
private ExpansionState src;
private Expansion_Master_Weapon_Unjamming_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master__Weapon_Unjamming_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master__Weapon_Unjamming_Transition_0";
Class.CastTo(src, _fsm.GetState("ExpansionState"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_Weapon_Unjamming_State_0"));
}
override int Guard() {
if (unit.IsInMelee()) return FAIL;	
if (!Class.CastTo(dst.weapon, unit.GetItemInHands())) return FAIL;	
if (!unit.GetWeaponManager().CanUnjam(dst.weapon)) return FAIL;	
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master_Weapon_Reloading_Idle_Transition_0 extends eAITransition {
private Expansion_Master_Weapon_Reloading_State_0 src;
private Expansion_Master_Idle_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master_Weapon_Reloading_Idle_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_Weapon_Reloading_Idle_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Master_Weapon_Reloading_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_Idle_State_0"));
}
override int Guard() {
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master_Weapon_Unjamming_Idle_Transition_0 extends eAITransition {
private Expansion_Master_Weapon_Unjamming_State_0 src;
private Expansion_Master_Idle_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master_Weapon_Unjamming_Idle_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_Weapon_Unjamming_Idle_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Master_Weapon_Unjamming_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_Idle_State_0"));
}
override int Guard() {
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master__Fighting_Transition_0 extends eAITransition {
private ExpansionState src;
private Expansion_Master_Fighting_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master__Fighting_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master__Fighting_Transition_0";
Class.CastTo(src, _fsm.GetState("ExpansionState"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_Fighting_State_0"));
}
override int Guard() {
if (unit.GetThreatToSelf() < 0.4) return FAIL;	
if (unit.GetActionManager().GetRunningAction()) return FAIL;	
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master_Fighting_Idle_Transition_0 extends eAITransition {
private Expansion_Master_Fighting_State_0 src;
private Expansion_Master_Idle_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master_Fighting_Idle_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_Fighting_Idle_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Master_Fighting_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_Idle_State_0"));
}
override int Guard() {
if (unit.GetThreatToSelf() > 0.2) return FAIL;	
if (unit.IsInMelee()) return FAIL;	
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master__Vehicles_Transition_0 extends eAITransition {
private ExpansionState src;
private Expansion_Master_Vehicles_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master__Vehicles_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master__Vehicles_Transition_0";
Class.CastTo(src, _fsm.GetState("ExpansionState"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_Vehicles_State_0"));
}
override int Guard() {
auto group = unit.GetGroup();	
if (!group) return FAIL;	
if (group.GetFormationState() != eAIGroupFormationState.IN) return FAIL;	
auto leader = group.GetLeader();	
if (!leader || leader == unit) return FAIL;	
if (!leader.IsInTransport()) return FAIL;	
Transport transport;	
if (!Class.CastTo(transport, leader.GetParent())) return FAIL;	
//TODO: make this event based instead and store as a variable within CarScript.	
//Prevents looping through the crew and insteads just compares a bool.	
for (int i = 1; i < transport.CrewSize(); i++)	
{	
if (transport.CrewMember(i) == null)	
{	
dst.seat = i;	
dst.entity = transport;	
return SUCCESS;	
}	
}	
return FAIL;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master_Vehicles_Idle_Transition_0 extends eAITransition {
private Expansion_Master_Vehicles_State_0 src;
private Expansion_Master_Idle_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master_Vehicles_Idle_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_Vehicles_Idle_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Master_Vehicles_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_Idle_State_0"));
}
override int Guard() {
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master__PlayEmote_Transition_0 extends eAITransition {
private ExpansionState src;
private Expansion_Master_PlayEmote_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master__PlayEmote_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master__PlayEmote_Transition_0";
Class.CastTo(src, _fsm.GetState("ExpansionState"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_PlayEmote_State_0"));
}
override int Guard() {
if (!unit.m_Expansion_EmoteID) return FAIL;	
if (unit.GetEmoteManager().IsEmotePlaying() || unit.GetEmoteManager().Expansion_GetCurrentGesture() == unit.m_Expansion_EmoteID) return FAIL;	
if (unit.GetThreatToSelf(true) > 0.2) return FAIL;	
if (unit.IsInMelee()) return FAIL;	
if (unit.GetWeaponManager().IsRunning()) return FAIL;	
if (unit.GetActionManager().GetRunningAction()) return FAIL;	
auto hands = unit.GetItemInHands();	
if (hands && (hands.IsInherited(BandageDressing) || hands.IsInherited(Rag)))	
return FAIL;	
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master_PlayEmote_Idle_Transition_0 extends eAITransition {
private Expansion_Master_PlayEmote_State_0 src;
private Expansion_Master_Idle_State_0 dst;
Expansion_Master_FSM_0 fsm;
void Expansion_Master_PlayEmote_Idle_Transition_0(ExpansionFSM _fsm) {
Class.CastTo(fsm, _fsm);
m_ClassName = "Expansion_Master_PlayEmote_Idle_Transition_0";
Class.CastTo(src, _fsm.GetState("Expansion_Master_PlayEmote_State_0"));
Class.CastTo(dst, _fsm.GetState("Expansion_Master_Idle_State_0"));
}
override int Guard() {
return SUCCESS;	
}
override ExpansionState GetSource() { return src; }
override ExpansionState GetDestination() { return dst; }
override string GetEvent() { return ""; }
}
class Expansion_Master_FSM_0 extends eAIFSM {
void Expansion_Master_FSM_0(ExpansionFSMOwnerType owner, ExpansionState parentState) {
m_Name = "Master";
m_DefaultState = "Expansion_Master_Idle_State_0";
Setup();
}
void Setup() {
AddState(new Expansion_Master_Idle_State_0(this));
AddState(new Expansion_Master_Unconscious_State_0(this));
AddState(new Expansion_Master_Trading_State_0(this));
AddState(new Expansion_Master_FollowFormation_State_0(this));
AddState(new Expansion_Master_TraversingWaypoints_State_0(this));
AddState(new Expansion_Master_Vehicles_State_0(this));
AddState(new Expansion_Master_Fighting_State_0(this));
AddState(new Expansion_Master_Weapon_Reloading_State_0(this));
AddState(new Expansion_Master_Weapon_Unjamming_State_0(this));
AddState(new Expansion_Master_TakeItemToHands_State_0(this));
AddState(new Expansion_Master_Bandaging_Self_State_0(this));
AddState(new Expansion_Master_PlayEmote_State_0(this));
AddTransition(new Expansion_Master__Unconscious_Transition_0(this));
AddTransition(new Expansion_Master_Unconscious_Idle_Transition_0(this));
AddTransition(new Expansion_Master__Trading_Transition_0(this));
AddTransition(new Expansion_Master_Trading_Idle_Transition_0(this));
AddTransition(new Expansion_Master__Bandaging_Self_Transition_0(this));
AddTransition(new Expansion_Master_Bandaging_Self_Idle_Transition_0(this));
AddTransition(new Expansion_Master_Idle_FollowFormation_Transition_0(this));
AddTransition(new Expansion_Master_Idle_TraversingWaypoints_Transition_0(this));
AddTransition(new Expansion_Master_TraversingWaypoints_Idle_Transition_0(this));
AddTransition(new Expansion_Master_FollowFormation_Idle_Transition_0(this));
AddTransition(new Expansion_Master__Weapon_Reloading_Transition_0(this));
AddTransition(new Expansion_Master__TakeItemToHands_Transition_0(this));
AddTransition(new Expansion_Master_TakeItemToHands_Idle_Transition_0(this));
AddTransition(new Expansion_Master__Weapon_Unjamming_Transition_0(this));
AddTransition(new Expansion_Master_Weapon_Reloading_Idle_Transition_0(this));
AddTransition(new Expansion_Master_Weapon_Unjamming_Idle_Transition_0(this));
AddTransition(new Expansion_Master__Fighting_Transition_0(this));
AddTransition(new Expansion_Master_Fighting_Idle_Transition_0(this));
AddTransition(new Expansion_Master__Vehicles_Transition_0(this));
AddTransition(new Expansion_Master__Vehicles_Transition_0(this));
AddTransition(new Expansion_Master_Vehicles_Idle_Transition_0(this));
AddTransition(new Expansion_Master__PlayEmote_Transition_0(this));
AddTransition(new Expansion_Master_PlayEmote_Idle_Transition_0(this));
}
}
ExpansionFSM Create_Expansion_Master_FSM_0(ExpansionFSMOwnerType owner, ExpansionState parentState) {
return new Expansion_Master_FSM_0(owner, parentState);
}
