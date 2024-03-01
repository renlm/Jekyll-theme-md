# Home
	A Jekyll theme for GitHub Pages.
	
### Jekyll
	https://www.jekyll.com.cn/docs/

### Git SSH Key
	$ git config --global user.name SpringCloudKubernetes
	$ git config --global user.email renlm@21cn.com
	$ ssh-keygen -t ed25519 -C "sck@github.com" -f ~/.ssh/id_sck
	$ curl -sfL https://renlm.gitee.io/docs/sh/GitSSHCfg.sh | HOST=github.com ALIAS=sck sh
	
	# 使用Host别名启用多SSH Key
	$ ssh -T git@sck
	$ git clone git@sck:SpringCloudKubernetes/Jekyll-theme-md.git
	
	# 复制公钥与私钥
	$ clip < ~/.ssh/id_sck.pub
	$ clip < ~/.ssh/id_sck

### Git Subtree
	$ git add .
	$ git commit -m 'Commit to add a subtree'
	$ git subtree add --prefix=assets/editor.md https://github.com/pandao/editor.md.git master --squash
	$ git subtree add --prefix=assets/mxgraph https://github.com/jgraph/mxgraph.git v4.2.2 --squash
	$ git push