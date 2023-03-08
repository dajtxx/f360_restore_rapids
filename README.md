# f360_restore_rapids

A modified Tormach PCNC1100 post processor to restore rapid moves.

This post processor analyses the move commands issued by F360 and replaces G1
commands with G0 where it is safe to do so - when the tool is moving to above
the stock top or making X/Y moves while above the stock top.
