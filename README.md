# iriuncam

Enable Multilib Repository: Ensure that the Multilib repository is enabled in your /etc/pacman.conf file.
Update Package Lists: Run the following command to update your package lists:
```
sudo pacman -Syu
```
Install Required Packages: Install prerequisites such as libnotify and gst-plugins-good:
```
sudo pacman -S libnotify gst-plugins-good
```
Install Iriun Webcam: Use yay to search for and install Iriun Webcam from the AUR:
```
yay -S iriunwebcam-bin
```
Remove and Reload v4l2loopback Module: If prompted by Iriun Webcam, remove and reload the v4l2loopback module:
```
sudo rmmod v4l2loopback
sudo modprobe v4l2loopback
```
Run Iriun Webcam: After installation and module reload, you should be able to run Iriun Webcam from the application menu or by executing its command in the terminal.
