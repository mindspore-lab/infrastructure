# infrastructure
一个用于在hub间（例如Github，Gitee）账户代码仓库同步的action定时任务仓库。

## 同步任务
1. github同步到gitee，除黑名单(infrastructure,awesome-nerf,mindformers)下的仓库全量同步(Mirror the github/mindspore-lab org repos to gitee/mindspore-lab).
src: github/mindspore-lab
dst: gitee/mindspore-lab
black_list: 'infrastructure,awesome-nerf,mindformers'


2. gitee同步到github，只白名单(mindformers)的仓库同步(Mirror the gitee/mindspore repos to github/mindspore-lab).
src: gitee/mindspore
dst: github/mindspore-lab
static_list: 'mindformers'
