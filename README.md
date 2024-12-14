# Fix-Windows11-Power-Plan-Problem-for-Armory-Crate
processor state 100% is not 100% unless you are using the plan is or of an duplicate of default "High Performance" power plan with GUID 8c5e7fda-e8bf-4a96-9a85-a6e23a8c635c

Go to Terminal:

POWERCFG/?

POWERCFG/L

POWERCFG/? /DUPLICATESCHEME

POWERCFG /DUPLICATESCHEME <SCHEME_GUID> [<DESTINATION_GUID>]

POWERCFG /DUPLICATESCHEME 8c5e7fda-e8bf-4a96-9a85-a6e23a8c635c 6fecc5ae-f350-48a5-b669-b472cb895ccf

the GUID 6fecc5ae-f350-48a5-b669-b472cb895ccf is the Turbo plan in Armory Crate

POWERCFG /CHANGENAME 6fecc5ae-f350-48a5-b669-b472cb895ccf "Turbo"
