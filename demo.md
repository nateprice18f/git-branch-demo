# Assuming you are on the main branch and have the latest changes 
```git checkout -b release-1.0 ```# Create a release branch  
```git checkout -b feature-1 release-1.0``` # Create a feature branch from the release branch 

# Make some changes and commit them on feature-1 
```git checkout -b feature-2 release-1.0``` # Create another feature branch from the release branch 

# Make some changes and commit them on feature-2 
```git checkout -b feature-3 release-1.0``` # Create another feature branch from the release branch 

# Make some changes and commit them on feature-3 
```git checkout release-1.0``` # Switch back to the release branch   
```git merge feature-1``` # Merge feature-1 into the release branch   
```git merge feature-2``` # Merge feature-2 into the release branch   

# Optionally, you can delete the merged feature branches 
```git branch -d feature-1 ```
```git branch -d feature-2```
