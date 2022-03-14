# Debian for Lulu
Dell Chromebook 13 7310 Lulu backlight

Copy xblight files to /usr/local/bin

Modify /etc/sudoers.d/backlight NOPASSWD

ALL ALL = (root:root) NOPASSWD: /usr/local/bin/dblight-\
ALL ALL = (root:root) NOPASSWD: /usr/local/bin/dblight+\
ALL ALL = (root:root) NOPASSWD: /usr/local/bin/kblight-\
ALL ALL = (root:root) NOPASSWD: /usr/local/bin/kblight+

Then open  Settings / Keyboard / Shortcuts

sudo dblight+    for F7\
sudo dblight-    for F6\
sudo kblight+    for Ctrl+F7\
sudo kblight-    for Ctrl+F6

amixer sset Master toggle      for F8\
amixer sset Master 5%-         for F9\
amixer sset Master 5%+         for F10\
