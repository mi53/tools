# tools
Cygwin

[diff]
    tool = jellybc3
[difftool]
    prompt = false
[difftool "jellybc3"]
    #use cygpath to transform cygwin path $LOCAL (something like /tmp/U5VvP1_abc) to windows path, because bc3 is a windows software
    cmd = \"/cygdrive/c/program files/Beyond Compare 4/bcomp.exe\" \"$(cygpath -w $LOCAL)\" \"$REMOTE\"
[merge]
    tool = jellybc3
[mergetool]
    prompt = false
[mergetool "jellybc3"]
    #trustExitCode = true
    cmd = \"/cygdrive/c/program files/Beyond Compare 4/bcomp.exe\" \"$LOCAL\" \"$REMOTE\" \"$BASE\" \"$MERGED\" \"$MERGED\"
[commit]
	template = /home/z00476673/.gitmsg


Ubuntu下xming乱码问题sudo apt-get install fonts-noto-cjk


[diff]
    tool = jellybc3
[difftool]
    prompt = false
[difftool "jellybc3"]
    #use cygpath to transform cygwin path $LOCAL (something like /tmp/U5VvP1_abc) to windows path, because bc3 is a windows software
    cmd = \"/usr/bin/bcompare\" \"$LOCAL\" \"$REMOTE\"
[merge]
    tool = jellybc3
[mergetool]
    prompt = false
[mergetool "jellybc3"]
    #trustExitCode = true
    cmd = \"/usr/bin/bcompare\" \"$LOCAL\" \"$REMOTE\" \"$BASE\" \"$MERGED\" \"$MERGED\"
[commit]
	template = /home/z00476673/.gitmsg
	
	
更新代码：
git add .;git stash;git pull;git stash apply 0
