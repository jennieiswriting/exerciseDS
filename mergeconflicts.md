## Sublime Merge

### Merge conflicts 
___
In most cases, Git automatically resolves and merges differences in code between two commits. However, if you merge two branches that contain competing code changes, Git cannot always automatically resolve the differences. This results in a merge conflict that requires your input.

Merge conflicts arise from different scenarios. Sometimes they occur because you edit a file that someone else has deleted. Most commonly, you—or you and a collaborator—modified the same file on the same line in two different branches:

<img width="615" width="417" alt="The summary pane displays competing commits, indicated by Git's standard conflict markers." src="https://github.com/user-attachments/assets/4ce5a38c-4f01-427a-858a-826e82b0c299">

You cannot resolve merge conflicts from only the Git command line. First, you must first tell Git which of the competing changes to keep in the final merged file. To resolve the conflict without using a merge tool, you can edit the merged file in your text editor or in GitHub's conflict editor. Both of these methods require that you manually remove Git's conflict markers: 
 `<<<<<<<`, `=======`, `>>>>>>>`.  

Sublime Merge simplifies merge conflict resolution with an interface that eliminates the need to manually edit the merged file.

<img width="766" height="333" alt="The merge tool UI displays two conflicting commits in separate panes next to a merged file pane in the middle." src="https://github.com/user-attachments/assets/ecaea09e-eadf-494c-b3a0-a6bd856ddb07">


#### Resolving a merge conflict in Sublime Merge
___
When you push a commit that causes a merge conflict, Sublime Merge highlights it in the **Summary** pane.

1. In the **Summary** pane, click **Resolve**.  
The **Merge Tool** opens.
2. Decide which commit to retain in the final merged file.  
The **Merge Tool** displays your most recent commit, the final merged file with a `CONFLICT` indicator, and the competing commit in three separate panes.  
3. Optional: to display the file as it exists in the base branch, click **Base**. Use the **Base** and **Merged** buttons to toggle between the `Base` and `Merged` files. 
4. Double-click the ▶ or ◀ pointers next to the final code that you want to merge.  
The selected code moves into the **`Merged`** file.  
5. Click **Save and Stage**.  
The **Merge tool** closes and returns you to the **Summary** pane.
6. Click **Commit merge**.  
