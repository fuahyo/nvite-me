# nvite-me

note:
git pull origin main --allow-unrelated-histories
git push -u origin main.

(kalau muncul ini:
To https://github.com/fuahyo/nvite-me.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/fuahyo/nvite-me.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
)
then:
git fetch origin
git merge origin/main
(kalau muncul ini:
fatal: You have not concluded your merge (MERGE_HEAD exists).
Please, commit your changes before you merge.
)
then:
git add .
git commit -m "Completed ongoing merge"
git merge origin/main
git push -u origin main
------------------------------------------
kalo muncul ini:
hint: core.useBuiltinFSMonitor will be deprecated soon; use core.fsmonitor instead
hint: Disable this message with "git config advice.useCoreFSMonitorConfig false"
hint: Disable this message with "git config advice.useCoreFSMonitorConfig false"
pakai ini:
git config advice.useCoreFSMonitorConfig false
------------------------------------------
