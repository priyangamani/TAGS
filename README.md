# TAGS

-------------------------------
1. What are tags / releases
2. Why should i create TAGs
3. When to create TAGs
4. How to create TAGs in git
     create | show | publish | delete

Step 1:
Checkout the branch where you want to create the tag
git checkout "branch name"
example : git checkout master
________________________________________________________

Step 2:
Create tag with some name
git tag "tag name"
example : git tag v1.0
git tag -a v1.0 -m "ver 1 of .."  (to create annotated tags) 
________________________________________________________

Step 3:
Display or Show tags
git tag
git show v1.0
git tag -l “v1.*”
________________________________________________________

Step 4:
Push tags to remote
git push origin v1.0
git push origin --tags
git push --tags 
(to push all tags at once)
________________________________________________________

Step 5:
Delete tags (if required only)
to delete tags from local :
git tag -d v1.0
git tag --delete v1.0

to delete tags from remote :
git push origin -d v1.0
git push origin --delete v1.0
git push origin :v1.0

to delete multiple tags at once:
git tag -d v1.0 v1.1 (local)
git push origin -d v1.0 v1.1 (remote)

________________________________________________________
