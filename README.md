# Team still there?
The project is divided into packages. Packages are associated to their teams via a reference in the package.json file found in the packages folder. However, teams can seize to be, or packages be moved to different teams. There is no guarantee that the package is removed, or the team reference in the package.json file.  


# How to accomplish this
1. Copy an example tree structure into this repository. 
2. Add package.json files in the valid places - ensure to rename packages. 
3. Create a hashmap for teams. Hashmap should have team names as key with an array the entry. 
4. Traverse the folder structure. For each team encountered, check if the team exists in the hashmap. If it does, add the package to the array associated to the key. If it doesn't, create a new entry in the hashmap with the team name as key and an array with the package as object. 
5. Expected outcome - print out the teams with their associated packages.