### Step 1.
  #### Create a new team in Teams (follow the hint) or use an existing Team’s team 😁
> Hint
![create team](/img/createTeam.png)
### Step 2.
  #### Create a channel. By default, a General channel will be created. Install the GitHub preview app in your Teams client (select the channel where you want to configure the app). Follow the hint.
> Hint

![create channel](/img/githubappinstall.png)

### Step 3. Join the Github repo (check step#2) assigned to your team. The repo has been configured with the below integrations. **Azure Boards and Azure Pipelines**
  #### Settings tab>Integrations
![ConfigBoardsPipelines](/img/ConfigBoardsPipelines.png)

### Step 4. Configure your GitHub repo to a **Teams channel**
  1. Navigate to the new Team created in Step #2
  2. Switch to the **General** Tab and start a new conversation ![new conversation](/img/newconversation.png)
  3. Type in @github and select the preview app installed in Step #2
  4. ![intellisenseone](/img/intellisenseGithubapp.png) when selected it should look like ![intellisensetwo](/img/intellisenseGithubapp-2.png) Refer to the table below to get a glimpse of the commands used in this lab

First Header | Second Header
------------ | -------------
@github signin | Connect to your GitHub Account. ![connected account](/img/githubaccountconnected.png) (you may get an error while installing the app asking for “organization owner” permissions. If so, please reach out to the host) 
@github subscribe orgname/reponame | Subscribe to your Organization and Repository. ![subToTeamRepo](/img/subToTeamRepo.png). Above notification features are enabled by default, and can be disabled with the @github unsubscribe owner/repo [feature] command: 1. issues - Opened / closed / ReOpened 2. pulls - New / merged / Close / ReOpen 3. commits - New commits on the default branch (usually master) 4. comments - New comments on issues and pull requests. **Subscribe to PR reviews (optional in steps to come)** @github subscribe orgname/reponame reviews ![subToTeamRepo](/img/subToTeamRepoReviews.png)

### Step 5. You may also subscribe to specific labels (not a part of this lab). Although, atm you cannot subscribe to ‘multiple’ labels.
  #### Refer this [link](https://github.com/integrations/microsoft-teams/blob/master/Readme.md#filters)


### Step 6. Let’s see how the notifications appear in the **Teams** channel. 
  1. Create a new branch.
  2. Navigate to Team-X/PartsUnlimited-aspnet45/README.md and edit the file
  3. Navigate to your Azure pipelines (add link here)
  4. Copy the build status badge from Azure pipelines
    i. Click on the last run of the Azure Devops pipeline
    ii. Navigate back the README.MD and add the sample markdown to the top of the file. Commit the change and check the Teams channel for notifications. There should  not be any notification, since the new branch is not the default branch on the repo. Master/base branch is the default branch.


### Step 7. Join the Github repo (check step#2) assigned to your team. The repo has been configured with the below integrations. **Azure Boards and Azure Pipelines**
  1. Navigate to the new Team created in Step #2
  2. Switch to the **General** Tab and start a new conversation ![create team](/img/)
