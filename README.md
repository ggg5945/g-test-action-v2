# g-test-action-v2

如果推送，但是没有任何更新，可以触发actions的执行吗

可以触发，但需要使用特定方法。

方法 1：空提交（推荐）

bash

git commit --allow-empty -m "Trigger workflow"

git push


travis-ci.com 收费
 master f62353f
 less than a minute ago
travis-ci 2
-
Owner ggg5945 is not on a new pricing.


https://app.circleci.com/home
docker方式部署的，需要保持前台运行不然会没有效果，先暂时不改了
30,000 credits/mo, that’s up to 6,000 build mins。每个月只有100小时的使用时间
0 GB of 1 GB used。每个月只有1G流量？



## 清理无用对象，减小git仓库大学
```
git reflog expire --expire=now --all
git gc --prune=now --aggressive
```



