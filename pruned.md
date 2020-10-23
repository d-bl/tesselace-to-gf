This project started as a pruned copy of https://github.com/d-bl/GroundForge
keeping only tesselace related content.

Many files moved a lot, so what to prune beyond the obvious was found
by trial and error while browsing through the remaining history.

It might not be the best approach according to https://git-scm.com/docs/git-filter-branch

    git filter-branch -f --tree-filter "rm -rf README.md build.sbt pom.xml project src toJS.bat toJS.sh 404.md API _config.yml docs/404.md docs/API docs/css docs/images docs/js docs/sheet.html docs/tiles.html docs/_includes/README.md docs/_includes/gallery.html docs/_includes/site-map.svg docs/_includes/stitches.html docs/help/A*.md docs/help/B*.md docs/help/C*.md docs/help/D*.md docs/help/F*.md docs/help/N*.md docs/help/P*.md docs/help/R*.md docs/help/S*.md docs/help/W*.md docs/help/Tr*.md docs/help/w docs/help/Undo.md docs/help/animation docs/help/bloopers docs/help/footside.html docs/help/images docs/help/index.md docs/help/stitches" --prune-empty HEAD 
    
    git filter-branch -f --tree-filter "rm -rf docs/includes/val* index.html *.js colorpicker *.png *.md target patterns images js debugD3js-v4 move-nodes docs/*.html docs/D3jsForcescss docs/README.md .travis.yml .github/PULL* .github/ISSUE* wiki* docs/animation bloopers docs/*.md docs/stitches stitches animation docs/help/Home.md docs/help/Para* help/examples/index.md help/examples/Droste* docs/help/Choose* docs/help/Thread* docs/help/Reshape* docs/help/examples/Droste* docs/_includes/stitch*  docs/help/*.png docs/help/*.gif *.html docs/help/examples/index.md docs/help/examples/stitch* docs/help/*NL* docs/help/M*.md docs/help/examples.md" --prune-empty HEAD 

    git filter-branch -f --tree-filter "rm -rf css/index.css docsD3js* docs/help/examples/Whi* docs/help/Tiles.md docs/_includes/val*" --prune-empty HEAD 
