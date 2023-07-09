# Add Git Repository Dataset 

You can a git repository as dataset source to this assistant and chat with this git repository. You can add mulitple repositories to this assistant, and chat with these repositories.
Also, you can remove any repository at any time you want to delete memory of this assistant without any effect on any other repositories/memories.
The total repositories you can attached is limited by your subscription plan.
We support both private and public repository as a dataset source.

### Attach Git Repository
1.  Click the avatar button in the right up corner of top navigation bar, in drop down menus, select My Assistants
2.  In your assistant dashboard, click the assistant name to navigate to assistant detail page.
3.  Click Dataset menu on left section, you can see the files learned by this assistant.
4.  Click 'Add dataset' button, Click 'Git Repository' tab
5.  On git reposiotry tab page, fill in the repository information
   + **Repository**: the git repository url, such as https://github.com/myusername/myproject.git
   + **Branch**: Only files in this branch will be learned.
   + **Directory**: the relative direcotry path in this repository, only files in this directory will be learned, such as /data, default is root directory in repository.
   + **File Excluded**: A regex pattern to filter out files by file name, files that match this pattern will not be trained.
   + **Extensions**: A regex pattern to filter out files by file extension, files that match this pattern will be trained.
   + **Account**: Optional, for private repository with user name and passowrd auth, this is the account name of this repository.
   + **Token**: Optional, for private repository with token auth, this is the access token, for user name and password auth, this is the password.

6.  Click 'Add' button to start tranning, we will process the git repository based on the rules defined here.
7.  Checkout the trainning status by click 'Refresh' button, When status of this dataset is in 'READY' state, you can now start chat conversation with this assistant.
8.  If any error occours, move mouse to the status field, the error message will be shown in tooltip.
9.  The Size field will display how much size of files in this repository processed, the Data trained field will show how much size(characters) learnd by LLM.
10. When you updated your repository, click 'Sync' icon button of this dataset, we will start syncing and learning new changes of this repository.
11. if you found an error, and caused by a ratelimit, don't worry, just start a sync procedure, the data already learned doesn't take into account of your subscription plan, and will be skipped.


### Why Data trained size is larger than the file size uploaded?

Due the embedding technology, for a new file, we will spilt your documents into text chunks at a fixed size. For better search result, we also add an overlap size to each chunk, the default overlap size is 10 bytes, thus the total data size trained will be the file size + total chunks * 10. The dataset limit in subscription plan is based on this value, total data trained size.


### Why Data trained size is 0 or smaller than file size uploaded?

We also use the cumulative value of all datasets uploaded to this assistant. For example, if you have two repositories, repo1 and repo2, and the content of repo2 is a clone or subset of repo1, so, in this case, when we detected a document chunk has been already learned by this assistant, the data trained size will not include this document chunk, only newly added document will be learned by assistant, so the data trained size only include newly learned document size. 

Note, when you delete a base dataset that referenced by other datasets of this assistant, the memory from this dataset will be earased, even though the other datasets may contains the same memory, so pay attation to the order of datasets of this assistant when removing.