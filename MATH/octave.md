```bash
$apt update -y
$apt upgrade -y
$apt install proot-distro -y
$proot-distro install debian
$proot-distro login debian
$apt update -y
$apt upgrade -y
$apt install octave -y
$octave --no-gui
octave:> x = 1:10;
y = x.^2;
plot(x, y);
title('Simple Grafik CLI');
octave:> quit
```
