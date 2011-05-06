Mirror of svn repository at http://svn.mulle-kybernetik.com/OCMock/trunk/

Created with these commands:

    mkdir OCMock
    cd OCMock
    git init
    git remote add origin git@github.com:jsheets/OCMock.git
    git svn init -s http://svn.mulle-kybernetik.com/OCMock
    git svn fetch
    git gc
    git push origin master

    git checkout -b svn trunk
    git push origin svn:refs/heads/svn
    git fetch origin
    git config branch.svn.remote origin
    git config branch.svn.merge refs/heads/svn

To update with latest svn commits:

    git checkout svn
    git svn rebase
    git push origin
    git checkout master
    git merge svn
