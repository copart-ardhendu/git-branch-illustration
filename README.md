
![image](https://user-images.githubusercontent.com/48975260/130593528-f9b31ff3-58cc-4c91-ac23-da1d9f07c0eb.png)

-	Master is the stable branch
-	Release-1 is the code which is present in prod
-	Release-2 is the code which is being planned for next release(next week)
-	Release-2 is currently being tested in QA
-	Requirement for release-3 is made available
-	Release-3 is built on top of release-2
-	There is an immediate requirement to patch the prod code, so we create a release-1.1
-	Another minor release is planned 1-day after the release-2 date, so we create a branch release-2.1 top of release-2
-	Requirement for release-4 is made available
-	Since development is going on other branches, developer decides to build on top of last prod release, keeping in mind the need to merge with master before deploying his changes for testing
 

# Next Incidents

![image](https://user-images.githubusercontent.com/48975260/130563550-955116d0-e6ce-4c8a-bbe4-f8ca6b2f8888.png)


-	Small requirement comes in, which is planned to be pushed in the current release
-	Code change could not be successfully tested in QA, so had to reverted, keeping in mind it needs to go in the next release
-	Emergency release-1.1 gets deployed to prod, and the branch is then merged to master
-	Release-2 gets deployed to prod, and its branch merged to master
-	Last Minute Change is put back in release-2.1, by doing revert(Revert)
-	This creates a merge conflict, which needs to be resolved
-	Release-2.1 gets deployed to prod, and its branch merged to master
-	For release-3, a compare with master gives the changes for the release
-	Release-3 gets deployed to prod, and its branch merged to master
-	Release-4 branch can be merged to master before being deployed for testing
 
# Rebase and Merge

![image](https://user-images.githubusercontent.com/48975260/130575494-b7a976d1-9955-405f-b45d-98964c033003.png)
 
