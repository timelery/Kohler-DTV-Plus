# Kohler-DTV-
Results of analyzing the Kohler DTV+ system controller and associated web page.

The Kohler DTV+ system controller (K-99695-NA and K-99693-P-NA) has an associated web page that is used to confogure the system components.

I spent some time looking into the web page and controller code and found a few useful pieces of information that would provie very useful if someone was inclined to interface withi this controller from another automation system.

By taking advantage of the discovered CGI scripts, someone could easily create a custom interface to manipulate the DTV+ components (Turn shower on, off, Turn on massage, Manipulate Audio or Lighting, etc).

None of this is documented by Kohler and as such such you will assume all responsibility for issues that may present themselves from interfacing with the controller in this way.

Here is a list of all CGI scripts I found that were coded into the controller. These can be executed by appending them to the end of the system controller url. For example: http://192.168.1.222/check_updates.cgi

Important: Through some initial testing I have found that some of these work and others do not. When some are executed the controller web page appears to freeze and a reboot is required. Proceed with caution. I will do some more digging and see if I can find details on whether or not any of the below cgi scripts require inputs and what those may be. Happy hacking!

check_updates.cgi
landing_url.cgi
mac.cgi
serial.cgi
clear_dt.cgi
files_available.cgi
reset_fault.cgi
saveDT.cgi
values.cgi
languages.cgi
rpc.cgi
datatable.cgi
edit_dt.cgi
set_device.cgi
swapvalves.cgi
unpack_bin.cgi
quick_shower.cgi
start_user.cgi
stop_user.cgi
light_on.cgi
light_off.cgi
music_on.cgi
music_off.cgi
steam_on.cgi
steam_off.cgi
rain_on.cgi
rain_off.cgi
id_interface.cgi
saveUI.cgi
reset_factory.cgi
forget_devices.cgi
reset_default.cgi
save_default.cgi
reset_users.cgi
reset_user.cgi
fileupload.cgi
BTKey.cgi
BTPin.cgi
save_variable.cgi
change_user.cgi
files.cgi
system_info.cgi
ftp_status.cgi
hiding.cgi
update_change.cgi
bt_disconnect.cgi
sim_dev_values.cgi
massage_toggle.cgi
powerclean_check.cgi
stop_shower



