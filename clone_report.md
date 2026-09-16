# Отчёт о клонировании чужого репозитория

## Ссылка на репозиторий
https://github.com/alibaba/open-code-review

## Вывод команды git log 

commit e556dfad56f11afe15cce9b1a0ca7f8993a65134 (HEAD -> main, origin/main, origin/HEAD)
Author: Ayush Dubey <ayushdubey3740@gmail.com>
Date:   Wed Sep 16 19:47:02 2026 +0530

    feat(viewer): align suggested change indentation with existing code gutter (#1313) (#1315)

    Align the Suggested Change code block with the Existing Code block when line numbers are displayed.

commit 6aa6dcd3c3a217db0a9fb84505f2ca20aa354a3e
Author: surefirestudios <surefirestudios2022@gmail.com>
Date:   Wed Sep 16 06:59:41 2026 -0700

    fix(diff): strip trailing CR from CRLF diff text (#1302)

    ParseDiffText and ParseHunks split on "\n" and kept the carriage return that
    CRLF-terminated diff text leaves on every line. It rode into the "diff --git"
    capture, so NewPath became "file.go\r" and the file could not be read for
    review, and it defeated the equality checks against "--- /dev/null", costing
    a diff its IsNew or IsDeleted flag.

    Fixes #933

    Co-authored-by: SurefireStudios <heresamemo@gmail.com>
    Co-authored-by: MeiSiristhebest <124799179+MeiSiristhebest@users.noreply.github.com>

commit f1101fd7f51304c82e4a4f292bbee88aea0823cf (tag: v1.12.4)
Author: DiegoCluv7 <161216254+iluv7@users.noreply.github.com>
Date:   Wed Sep 16 17:48:17 2026 +0800

    perf(diff): skip oversized untracked files before reading (#1310)

commit afdd883fc7235b9db6bd3307b7168fd67fc42dc0
Author: xiaodu55 <1704788159@qq.com>
Date:   Wed Sep 16 17:14:52 2026 +0800

    fix(diff): flag untracked binary files as binary in workspace mode (#1288)

commit e81d80146c12cf379c9bc4389abeec86e6d9c925
Author: Kite <254839944+lizhengfeng101@users.noreply.github.com>
Date:   Wed Sep 16 17:04:46 2026 +0800

    test(action): satisfy resolved_head contract in workflow_run pr_number test (#1309)

    The #1156 test posted inline comments on a workflow_run event without a
    manifest, tripping the input.resolved_head requirement that landed on main
    in parallel. Provide a manifest so the test exercises the intended path.

commit 042c382c73d0b347c964281046aae2fed292fd1e
Author: Doksanbir <ylcn91@users.noreply.github.com>
Date:   Wed Sep 16 11:37:28 2026 +0300

    feat(action): add optional pr_number input and workflow_run fallback (#1156)

    * feat(action): add optional pr_number input and workflow_run fallback


## Вывод команды git shortlog -sn

   250  kite
    35  chethanuk
    29  Tao Xin
    23  Kite
    23  Lei Zhang
    13  xujiejie
    12  祈愿Qiii
    11  Abdul Moiz Hussain
    11  dependabot[bot]
    10  Gongyl01
     9  MuoDoo
     8  hezheng.lsw
     8  wxwxwxw_orange
     6  Minsu Lee
     6  不许对我狗叫丶
     6  林SO
     6  超級の新人
     5  Ben Younes
     5  c
     5  xyJen
     4  Hao Guo
     4  Nefelibata
     4  Nitish Agarwal
     4  Qiaochu Hu
     4  Shaurya Srivastava
     4  zhouzhihao
     3  A
     3  Fanzzzd
     3  LKL-ZREO
     3  Ritvik K
     3  ScarletCarpet
     3  Sisanta Chhatoi
     3  Zhiming Wang
     3  hyy
     3  munsunouk
     3  nolanchic
     3  pablo
     3  zephyrq-z
     2  Ayrton
     2  Ayush Pandey
     2  BASIL K AJI
     2  DiegoCluv7
     2  Do Tuan Anh
     2  Eldar Shlomi
     2  Fedor
     2  FenjuFu
     2  Hyeseong Kim
     2  Jiale Li
     2  Luis Rodriguez
     2  Magnus
     2  Parikalp Bhardwaj
     2  Polly Labs
     2  Praveen Kumar Mittal
     2  Roc
     2  Shi Peipei
     2  Syt3s

