// Optimised CS2 Autoexec – generated 2025‑07‑16
echo "Optimised autoexec.cfg loaded – top‑UK coach edition"

// === Mouse & Sensitivity ===

m_rawinput "1"                    //Enable Raw Input for perfect precision (Raw input is unavailable on OSX)
m_mouseaccel2 "0"                 //Disables windows mouse acceleration initial threshold, safety precaution
m_mouseaccel1 "0"                 //Disables windows mouse acceleration initial threshold, safety precaution
m_customaccel "0"                 //Custom mouse acceleration disabled
zoom_sensitivity_ratio_mouse 0.8189
sensitivity "2.13"                //Adjust to preference //DPI 400
zoom_sensitivity_ratio "0.8189330271"

// === Viewmodel ===

viewmodel_fov "68"
viewmodel_offset_x "2"    //Changes viewmodel view in X scale (-2 to 2.5)
viewmodel_offset_y "0"    //Changes viewmodel view in Y scale (-2 to 2)
viewmodel_offset_z "-1.5" //Changes viewmodel view in Z scale (-2 to 2)

// === Crosshair (huNter‑ 2025) ===
// Code: CSGO-wTm8n-xyNG7-Gedpn-BS9MO-TpNkO
cl_crosshairgap "-3"
cl_crosshair_outlinethickness "1"
cl_crosshaircolor_r "255"
cl_crosshaircolor_g "255"
cl_crosshaircolor_b "255"
cl_crosshairalpha "255"
cl_crosshair_dynamic_splitdist "3"
cl_crosshair_recoil "false"
cl_fixedcrosshairgap "-2"
cl_crosshaircolor "2"
cl_crosshair_drawoutline "1"
cl_crosshair_dynamic_splitalpha_innermod "0"
cl_crosshair_dynamic_splitalpha_outermod "1"
cl_crosshair_dynamic_maxdist_splitratio "1"
cl_crosshairthickness "1"
cl_crosshairdot "0"
cl_crosshairgap_useweaponvalue "0"
cl_crosshairusealpha "1"
cl_crosshair_t "0"
cl_crosshairstyle "4"
cl_crosshairsize "1"

// === Custom Binds ===
bind "LEFTARROW" "+turnleft"
bind "RIGHTARROW" "+turnright"
bind "UPARROW" "+forward"
bind "DOWNARROW" "+back"
bind "ENTER" "+attack"


// === Netcode ===
rate "786432"                     // 6.2 Mbps – safe high value
cl_updaterate "128"
cl_cmdrate "128"
cl_interp "0.015625"
cl_interp_ratio "1"
cl_lagcompensation "1"

// === Performance ===
fps_max "400"                     // cap to keep frametimes stable
fps_max_ui "0"
engine_low_latency_sleep_after_client_tick "true"
vprof_off
r_csgo_water_refraction "0"
r_csgo_water_effects "0"

// === QoL & HUD ===
cl_radar_always_centered "1"
cl_hud_color "8"                  // team colour
cl_showfps "0"
net_graph "1"

// === Binds ===
bind "f" "+voicerecord"           // push‑to‑talk
bind "mouse5" "use weapon_knife;use weapon_flashbang"       // quick‑flash
bind "space" "+jump"
bind "mwheeldown" "+jump"

//=== Hands ===
cl_righthand 0
bind "leftarrow" "cl_righthand 0"
bind "rightarrow" "cl_righthand 1"

// === Aliases ===
alias "rs" "mp_restartgame 1"

// Launch Options 
//-console -nojoy +fps_max 0 -softparticlesdefaultoff \
//-fullscreen -refresh 240 -forcenovsync \
//+engine_low_latency_sleep_after_client_tick true

//------------------------------------------
/------------------------------------------
// Alternative Command Script - by MrMaxim
// Hold down a toggle key to trigger a secondary command	 
// Part 1 (Input Primary/Default Command)
alias defZ		"bind z radio"
alias defX		"bind x slot12"
alias defC		"bind c radio2"
alias defQ		"bind q lastinv"
alias defE		"bind e +use"
alias defF		"bind f +voicerecord"
alias defG		"bind g drop"
alias def1		"bind 1 slot1"
alias def2		"bind 2 slot2"
alias def3		"bind 3 slot3"
alias defP		"bind p say gg"

// Part 2 (Make sure the keyboard letters are the same as part 1)
alias keyZ		"bind z customZ"
alias keyX		"bind x customX"
alias keyC		"bind c customC"
alias keyQ		"bind q customQ"
alias keyE		"bind e customE"
alias keyF		"bind f customF"
alias keyG		"bind g customG"
alias key1		"bind 1 custom1"
alias key2		"bind 2 custom2"
alias key3		"bind 3 custom3"
alias keyP		"bind p customP"

// Part 3 (Input Secondary Command)
alias customZ	"god"
alias customX	"noclip"
alias customC	""
alias customQ	"use weapon_flashbang"
alias customE	"use weapon_hegrenade"
alias customF	""
alias customG	""
alias custom1	"use weapon_smokegrenade"
alias custom2	"use weapon_molotov; use weaponinc_grenade"
alias custom3	"use weapon_decoy"
alias customP	"sv_grenade_trajectory_prac_pipreview 1; sv_grenade_trajectory_prac_trailtime 4; mp_buy_anywhere 1; mp_freezetime 0; mp_ignore_round_win_conditions 1; mp_buytime 99999; mp_startmoney 60000; mp_maxmoney 60000; ; ammo_grenade_limit_total 6; mp_warmup_pausetimer 1; mp_warmup_start; sv_cheats 1; sv_infinite_ammo 2; bot_kick; say Practice Enabled"

//Part 4 (Don't touch, wierdo)
alias +secondarycommand "keyZ; keyX; keyC; keyQ; keyE; keyF; keyG; key1; key2; key3; keyP"
alias -secondarycommand "defZ; defX; defC; defQ; defE; defF; defG; def1; def2; def3; defP"

//Part 5 (Toggle - Holding this will trigger your secondary commands)
bind alt +secondarycommand



host_writeconfig
