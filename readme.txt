
这个存储库用来收集陷阱公司，如果你遇到哪个公司强制加班，拖欠工资，职场霸凌等等损害劳动者权益的情况，就可以把那家公司放进这个存储库里。

一家公司一个文件，文件名用公司名命名，即可能的采用txt纯文本方式，如果要采用html等富文本方式，需要将这个文件对应的css、图片、等放进 对应的公司名.d/ 这样命名方式的文件夹中，避免全摊在根路径，以免被别人覆盖掉。




任何人都可以向我们提出 pull request .
操作方式如下：

--> 如果你已经被加入到了协作者列表中的话，请按下面的步聚提出 pull request :
git clone git@github.com:evil-trap/trapcompany.git
git checkout -b <你将来要提交PR的分支名称，比如：my-feature>
git diff
git add <changed_files>
git commit -m "提交描述，尽量做到言简意赅，以免被repo误认为是垃圾提交"
git push origin my-feature

----> 如果提交时发现 main 分支有了新的commit更新，就多做这几步：
git checkout main
git pull origin master
git checkout my-feature
git rebase main
有可能会出现 rebase conflict
这时需要一个个手动选择保留哪一行
git push -f origin my-feature



--> 如果你还没有被加入到协作者列表中的话，就用下面的方式提出 pull request :
用浏览器打开存储库网址
https://github.com/evil-trap/trapcompany
在右上部找到 Fork 按钮就点击
这样做的目的是为了让你获得一个有完整权限的存储库。所以你可以想怎么改就怎么改。
改完之后，先推回(push)到你自己的存储库中。就是你刚才fork回来的那个有完整权限的repo中
然后就可以在你自己的github账户中找到那个fork回来的repo，你会在绿色的 <>Code 按钮下边靠左一点看到一个 Contribute 按钮，点它你就会看到绿色的 Open pull request 按钮了，点它就能提出 PR 了
如果我们觉得可以合并进main的话，你就会在我们做完merge后收到邮件通知和github的站内通知。
之后你可以选择删掉你fork的repo,这样就不会在下次提交PR时导致分不清的情况了。同时这也会减掉我们主repo的Fork的数值，所以我们并不是以此来增加fork量的。







