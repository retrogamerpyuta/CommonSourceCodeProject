# CommonSourceCodeProject

Toshiya Takedaさんの Common Source Code Projectに変更を加えたものです。\
kuran-kuranさんのリポジトリからForkしています。

＜変更点＞\
2026/09/16　EmuZ-80Kのサウンドのテンポが実機より遅いと感じたため修正。\
・MZ-80では、テンポ（音長）調整は、ソフトウェア制御で、CPUクロック数による遅延処理で行っているようだ\
・そこで、memory.cpp　の　EVENT_TEMPOのクロック数を整数倍で調整する方針とした。\
・感覚的には、「調整済みの実機の1.2～1.3倍くらいに間延びしている」と考え、32Hz*2→32Hz*3に変更。
