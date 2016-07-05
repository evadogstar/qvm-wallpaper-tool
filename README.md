# qvm-wallpaper-tool
convert images at the remote appVm to make them secure then downalod them to dom0 then convert it 2 time the same way

Store it at dom0 then chmod +x it then

`qvm-wallpaper-tool <appVM> {path_to_jpg_or_png} 

### Under the hood:
0. Convert image at AppVM with ImageMagick and store it with new temp name at AppVM
0. Download converted image to dom0 temp
0. Convert it 2(next) time at dom0 to prevent maybe possible injections at AppVM

### Issues
* No without GUI
* It's only works with jpg and png filenames at remote AppVM (for securety reasons)
* It do not set wallpapers. Only store them at user Pics directory (do not know how to set wallpapers, I tied some code and it does not work)
* 

