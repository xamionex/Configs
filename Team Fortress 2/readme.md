# Please read the autoexec

## How to install
1. Download\
![image](https://github.com/xamionex/Configs/assets/57235791/da027cb2-c086-470a-a1ec-5be8215e50ec)
2. Locate TF2 location\
![image](https://github.com/xamionex/Configs/assets/57235791/c49d6d46-26e8-4d4e-8f06-5731e57ef2c4)
3. Go into Team Fortress 2/tf/cfg/\
![image](https://github.com/xamionex/Configs/assets/57235791/3ecdeba7-887f-402a-8bd9-c44a5075ea1e)
![image](https://github.com/xamionex/Configs/assets/57235791/74fa488a-7bcc-4dbc-adad-e564c882349f)
4. Extract the zip into the folder (using 7zip)\
![image](https://github.com/xamionex/Configs/assets/57235791/27e5f31c-2a7a-4a95-85bd-3ee7a72ad911)
5. IF Ingame: run `exec autoexec` in console
   - If console is disabled either:
     - go into options > controls > advanced > enable developer console, then open it with ~
     - restart the game

### A lot of the things in this cfg are explained inside there, here are some previews though

![image](https://github.com/xamionex/Configs/assets/57235791/e5a159fd-6284-41d1-b3d8-1331d4fe0ff6)
![image](https://github.com/xamionex/Configs/assets/57235791/6f3f19d7-0daa-4ada-be3f-7cd7dac546e4)
![image](https://github.com/xamionex/Configs/assets/57235791/2fe07026-0264-4d6b-b392-96e2a170da1f)
![image](https://github.com/xamionex/Configs/assets/57235791/dfd8c0ca-c25f-4f7c-ad05-9158afa11342)

### Default cfg settings
```
NETWORK 
--------------------------------------------------------------------------------------------------- 
  
"cl_updaterate" = "66" ( def. "20" )
** NOTE: The real value is 100.000 but the server has temporarily restricted it to 66.000 **
 archive notconnected
 - Number of packets per second of updates you are requesting from the server
  
"cl_cmdrate" = "100" ( def. "30" ) min. 10.000000 max. 100.000000
 archive
 - Max number of command packets sent to server per second
  
"rate" = "100000" ( def. "80000" )
 archive
 - Max bytes/sec the host can receive data
  
"cl_resend" = "1.5" ( def. "6" ) min. 1.500000 max. 20.000000
 - Delay in seconds before the client will resend the 'connect' attempt
  
"cl_lagcompensation" = "1"
 client notconnected
 - Perform server side lag compensation of weapon firing events.
  
"cl_interp_ratio" = "1" ( def. "2.0" )
** NOTE: The real value is -1.000 but the server has temporarily restricted it to 1.000 **
 client archive notconnected
 - Sets the interpolation amount (final amount is cl_interp_ratio / cl_updaterate).
  
"cl_interp" = "0.033000" ( def. "0.1" ) min. 0.000000 max. 0.500000
 client archive notconnected
 - Sets the interpolation amount (bounded on low side by server interp ratio settings).
  
--------------------------------------------------------------------------------------------------- 
  
cl_interp explanation : 
  
Low interpolation values make your view more accurate, but less smooth. Moving objects may teleport around or may not be easy to follow, depending on your connection and the server tickrate. 
High interpolation values make your view less accurate, but smoother. Hitboxes will be ahead of their models. 
  
--------------------------------------------------------------------------------------------------- 
TEXTURES 
--------------------------------------------------------------------------------------------------- 
  
"mat_mipmaptextures" = "0" ( def. "1" )
  
"cl_detailfade" = "0" ( def. "400" )
 - Distance across which detail props fade in
  
"cl_detaildist" = "0" ( def. "1200" )
 - Distance at which detail props are no longer visible
  
"r_drawdetailprops" = "0" ( def. "1" )
 - 0=Off, 1=Normal, 2=Wireframe
  
"mp_decals" = "0" ( def. "200" )
 archive
  
"r_decals" = "0" ( def. "2048" )
  
--------------------------------------------------------------------------------------------------- 
PROPS 
--------------------------------------------------------------------------------------------------- 
  
"cl_phys_props_enable" = "0" ( def. "1" )
 client
 - Disable clientside physics props (must be set before loading a level).
  
"cl_phys_props_max" = "0" ( def. "300" )
 client
 - Maximum clientside physic props
  
"props_break_max_pieces" = "0" ( def. "-1" )
 - Maximum prop breakable piece count (-1 = model default)
  
"r_propsmaxdist" = "1" ( def. "1200" )
 client
 - Maximum visible distance
  
--------------------------------------------------------------------------------------------------- 
RAGDOLLS 
--------------------------------------------------------------------------------------------------- 
  
"g_ragdoll_fadespeed" = "600"
 client
  
"g_ragdoll_lvfadespeed" = "100"
 client
  
"ragdoll_sleepaftertime" = "5.0f"
 client
 - After this many seconds of being basically stationary, the ragdoll will go to sleep.
  
"cl_ragdoll_fade_time" = "15"
 client
  
"cl_ragdoll_forcefade" = "0"
 client
  
"cl_ragdoll_physics_enable" = "1"
 client
 - Enable/disable ragdoll physics.
  
--------------------------------------------------------------------------------------------------- 
GRAPHICS 
--------------------------------------------------------------------------------------------------- 
  
"mat_queue_mode" = "2" ( def. "-1" )
 archive
 - The queue/thread mode the material system should use: -1=default, 0=synchronous single thread, 2=queued multithreaded
  
"lod_TransitionDist" = "-1" ( def. "800" )
 client
  
"r_lod" = "2" ( def. "-1" )
  
"r_shadows" = "0" ( def. "1" )
  
"mat_hdr_level" = "0" ( def. "2" )
 archive
 - Set to 0 for no HDR, 1 for LDR+bloom on HDR maps, and 2 for full HDR on HDR maps.
  
"mat_vsync" = "0" min. 0.000000 max. 1.000000
 - Force sync to vertical retrace
  
"mat_dxlevel" = "95" ( def. "0" )
 singleplayer
 - Current DirectX Level. Competitive play requires at least mat_dxlevel 90
  
"tf_enable_glows_after_respawn" = "0" ( def. "1" )
 client archive
 - Enable teammate glow effects after respawn.
  
--------------------------------------------------------------------------------------------------- 
```
