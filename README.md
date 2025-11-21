# g-test-action-v2

如果推送，但是没有任何更新，可以触发actions的执行吗

可以触发，但需要使用特定方法。

空提交
```bash
git commit --allow-empty -m "Trigger workflow"
git push
```


## travis-ci.com 收费
```
 master f62353f
 less than a minute ago
travis-ci 2
-
Owner ggg5945 is not on a new pricing.
```

## https://app.circleci.com/home
```
docker方式部署的，需要保持前台运行不然会没有效果，先暂时不改了
30,000 credits/mo, that’s up to 6,000 build mins。每个月只有100小时的使用时间
0 GB of 1 GB used。每个月只有1G流量？
```


## 清理无用对象，减小git仓库大小
```
git reflog expire --expire=now --all
git gc --prune=now --aggressive
```


## 按Tab无提示问题
```
会优先使用 bash，如果不存在则回退到 sh
$(command -v bash || command -v sh)
但是实际测试不能切换到其他目录

后续通过ttyd ./init_ttyd.sh启动，在init_ttyd.sh直接bash，可以切换目录，也有提示了
```
