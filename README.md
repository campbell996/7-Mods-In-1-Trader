# 7-Mods-In-1.-Trader-Master
This Download Includes.    @Flying Circus <> @Flying Machines <> @HMCS Addon <> @Military Aviation <> @Sab Civil Aviation <> @Secret Weapons <> @Walkers A2 Vehicles <

This Installation Requires 7 Mods:
1. https://steamcommunity.com/sharedfiles/filedetails/?id=756357175
2. https://steamcommunity.com/sharedfiles/filedetails/?id=756348635
3. https://steamcommunity.com/sharedfiles/filedetails/?id=756352410 
4. https://steamcommunity.com/sharedfiles/filedetails/?id=756347016
5. https://steamcommunity.com/sharedfiles/filedetails/?id=938711359
6. https://steamcommunity.com/sharedfiles/filedetails/?id=952560410
7. https://steamcommunity.com/sharedfiles/filedetails/?id=1103511215
  
This File Is Better To Read In Notepad++. 

This is the Exile trader files for > @FlyingCircus <> @FlyingMachines <> @HMCSAddon <> @MilitaryAviation <> @SabCivilAviation <> @SecretWeapons <> @WalkersA2Vehicles <
DOWNLOAD>>>>>  <<<<< DOWNLOAD
 
I Did Not create These Mods. But I Did Create These Trader Files. 

INSTALLATION 

Step 1. Using pbo manager extract your mission.pbo & enter the mission folder that is extracted.   http://www.armaholic.com/page.php?id=16369 

Step 2. Create a folder called >>>>> traders <<<<<. Continue on step 3. 

Step 3. Place the >>>>> 7IN1 <<<<< folder that comes with this download. In the traders folder from step 2. 

Step 4. Open your >>>>> config.cpp <<<<< file using notepad++. Continue on step 5. 

Step 5. Find >>>>> class CfgExileArsenal <<<<< and add this at the top >>>>> #include "traders\7IN1\ItemList7IN1.hpp" <<<<<.

Step 5 Example

This is what it is before.

////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
class CfgExileArsenal
{
 class Exile_Uniform_BambiOverall    { quality = 1; price = 1; sellPrice = 1; };
 ///////////////////////////////////////////////////////////////////////////////
 // Civillian Clothing
 ///////////////////////////////////////////////////////////////////////////////
 class U_C_Journalist        { quality = 1; price = 20; };
 class U_C_Poloshirt_blue       { quality = 1; price = 20; };
 
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

And this is what it should be after...

class CfgExileArsenal
{
 #include "traders\7IN1\ItemList7IN1.hpp"
 class Exile_Uniform_BambiOverall    { quality = 1; price = 1; sellPrice = 1; };
 ///////////////////////////////////////////////////////////////////////////////
 // Civillian Clothing
 ///////////////////////////////////////////////////////////////////////////////
 class U_C_Journalist        { quality = 1; price = 20; };
 class U_C_Poloshirt_blue       { quality = 1; price = 20; };
 
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
 
 
Step 6. Find >>>>> class CfgTraderCategories <<<<< and add this at the top >>>>> #include "traders\7IN1\TraderCategories7IN1.hpp" <<<<<.

Step 6 Example

This is what it is before.

////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
class CfgTraderCategories
{
 class Community
 {
  name = "Community Items";
  icon = "a3\ui_f\data\gui\Rsc\RscDisplayArsenal\uniform_ca.paa";
  items[] =
  {
 
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

And this is what it should be after.

class CfgTraderCategories
{
 #include "traders\7IN1\TraderCategories7IN1.hpp"
 class Community
 {
  name = "Community Items";
  icon = "a3\ui_f\data\gui\Rsc\RscDisplayArsenal\uniform_ca.paa";
  items[] =
  {
 
//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////// 

Step 7. Find >>>>> class CfgTraders <<<<< And in that Find >>>>> class Exile_Trader_Vehicle <<<<<

and add both of these >>>>> >"HMCSRobots",<>"WalkersA2Cars"< <<<<<. 

Step 7 Example

This is what it is before.

////////////////////////////////////////////////////////////////////
class Exile_Trader_Vehicle
 {
  name = "VEHICLE";
  showWeaponFilter = 0;
  categories[] =
  {
   "Cars",
   "Trucks"
  };
 };
////////////////////////////////////////////////////////////////////

And this is what it should be after...   Dont forget the last catrgory cant have a > , <   but the rest must.

class Exile_Trader_Vehicle
 {
  name = "VEHICLE";
  showWeaponFilter = 0;
  categories[] =
  {
   "Cars",
   "Trucks",
   "HMCSRobots",
   "WalkersA2Cars"
  };
 };
////////////////////////////////////////////////////////////////////// 

Step 8. Find >>>>> class CfgTraders <<<<< And in that Find >>>>> class Exile_Trader_Aircraft <<<<<
and add this >>>>> > "SABChoppers",<>"SABPlanes" <<<<< Same as above example. except in the >>>>> class Exile_Trader_Aircraft <<<<<. 

Step 9. Download All 7 Of These Mods >>>>> @Flying Circus <> @Flying Machines <> @HMCS Addon <> @Military Aviation <> @Sab Civil Aviation <> @Secret Weapons <> @Walkers A2 Vehicles<<<<< from either the A3Launcher or from the Steam Workshop.
 
Step 10. Copy All 7 Of The Mods You Just Downloaded And Add Them To Your Exile Server Root Folder. And Remove All Spacing In The Folders Names.

Step 10 Example      BEFORE: @HMCS Addon   AFTER: @HMCSAddon
 
Step 11. Add the Bikey's to your server keys folder. If Required.
 
Step 12. Add >>>>> @FlyingCircus;@FlyingMachines;@HMCSAddon;@MilitaryAviation;@SabCivilAviation;@SecretWeapons;@WalkersA2Vehicles; <<<<< to your server start parameter. 


Enjoy........
