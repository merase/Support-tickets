# Support-tickets

### **Ticket 1: Rejected pull request from fork**
_**To start, I have to say I LOVE GITHUB. You guys rock. I was at your 4th birthday party,
thanks for the cupcake and booze!
Anyway, here's my problem. I sent a pull request to technoweenie, and he rejected it because
my master branch is out of sync with his master. What can I do to fix this?
Help me supportocat, you're my only hope!
/.Steve
Hint: You'll want to address their question, and you could add an explanation of topic
branches as a better workflow.**_

### **Ticket 1 response:**
Hi Steve,
      
Thank you for contacting GitHub support, I am Michael from the support team and I will be taking over the resolution of this ticket.
First, you do not want to lose the commit that you did so you cannot do a git hard reset to a prior sha. You will put your changes on a new branch and reset the master branch back to match the upstream by following below steps.

1. Move the last commit to a new branch
* git branch newbranch
* git reset --hard HEAD~1 # Go back 1 commit or use SHA
* git checkout newbranch

2. Resync your Github fork
* git checkout master
      
Since you already pushed this branch to your Github fork, you will see the message that contains your fix:
**"Your branch is behind 'origin/master' by 1 commit, and can be fast-forwarded."**

3. Fetch the branches and their respective commits from the upstream repository. Commits to master will be stored in a local branch, upstream/master by using below command.
* git fetch upstream

4. Checkout your fork's local master branch using below command.
* git checkout master

5. Merge the changes from upstream/master into your local master branch. This brings your fork's master branch into sync with the upstream repository, without losing your local changes.
* git merge upstream/master

6. your local master should Fast-forward to match the upstream. All is good, except your repo on Github is not correct as it contains your original commit on the wrong branch.
* git push --force

Below are some useful links regarding syncing of forks and working with branches
* [Syncing a fork](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/syncing-a-fork)
* [Commit a Branch fork](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/committing-changes-to-a-pull-request-branch-created-from-a-fork)
* [Branches](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-branches)
            
I look forward to hearing back from you soon. If you have any questions or concerns kindly let me know and I will be happy to address them.

regards,

Michael M.

GitHub Support.

***
### **Ticket 2: Syncing internal server and GitHub?**
_**Hi GitHub! My company has an internal Git server used for deployments, we use GitHub,
and I work on a local copy of the repository. For workflow purposes, how do I sync my
repository to GitHub and the internal Git server?
Thanks,
vmg
Hint: One common option is Git remotes. There are others!**_

### **Ticket 2 response:**
Hi VMG,

Thank you for reaching out to GitHub, My name is Michael and I shall be taking ownership of this ticket.

In this scenario, there are a couple of options;
1. GitHub Repo Sync Option which allows syncing with the current repository. For a step by step guide on how to use this option kindly check this link for the [GitHub Repo Sync](https://github.com/marketplace/actions/github-repo-sync).

2. Git Sync Action option which allows pushing to a remote repository. For a step by step guide on how to use this option kindly check this link for the [Git Sync](https://github.com/marketplace/actions/git-sync-action).

3. GitHub Desktop option which provides a GUI. For a step by step guide on how to use this option kindly check this link for the [GitHub Desktop](https://help.github.com/en/desktop/contributing-to-projects/syncing-your-branch).

4. Git Remote option via CLI. For a step by step guide on how to use this option kindly check this link for the [Git Remote](https://help.github.com/en/github/using-git/adding-a-remote) and [Git Remote fork](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/configuring-a-remote-for-a-fork).

Kindly check either of the above options. Please don't hesitate to let us know if you have any questions or concerns.

regards,

Michael M.

GitHub Support.

***

### **Ticket 3: Unhappy about forking**
_**JamesTK here, I have another question.
One of my dev collaborator forked my private repo without explicit permission to do so... is
that typical? I am surprised that the system did not notify me if it was okay to grant the fork
permission. Is there a way to setup permissions of this sort? Also, other than asking the
collaborator to delete the forked repo, can I actually delete it?
Thanks, jamestk
Notes:
You've checked the account in our admin view, he only has one personal repository
(jamestk/tribbles), which has one collaborator. Any documentation you may need is available
on help.github.com.**_

### **Ticket 3 response:**
Hi James,

Thank you for contacting GitHub support. 

In a private repository like yours, repository owners can only grant write access to collaborators. Collaborators cannot have read-only access to repositories owned by a user account hence this is the reason your Dev collaborator was able to fork your private repo.

More information about permission levels for a repository owned by a user account can be found on this GitHub [link](https://help.github.com/en/github/setting-up-and-managing-your-github-user-account/permission-levels-for-a-user-account-repository).

Since your repository is private, you can also delete the forked repository and this will delete all of its forks. For more information on this, kindly check out the knowledge base article on this GitHub [link](https://help.github.com/en/github/administering-a-repository/deleting-a-repository).

Please don't hesitate to let us know if you have any questions or concerns. Thank You.

regards,

Michael M.

GitHub Support.

***
## **Love to know more about yourself**
*We'd also love if you could share more about yourself so the team can get to know you
better! If you could fill the following out that would be great:*

#### **Name?**
Michael Machuka

#### **Location?**
Nairobi, Kenya. (The Green City In The Sun)

#### **What's an impressionable experience you've had with customer service/support, and why?**
I had the please of working with a customer from one of the companies I was supporting, we had just rolled out a new product which was new to the African market. For the product to be receptive and for the subscribers and merchants to accept it, there needed to be numerous training and material preparation to train the support engineers at the customer site. I took upon the challenge to personally create this training material then schedule a 2-hour session every evening with the engineers to train them so that they could ramp up their knowledge on the product then be able to assist the subscribers and merchants in the field using the product. I was not tasked to do the training but out of my own personal passion to better other individuals, I took upon this task to train them, in the process enhance my knowledge on the product as well. This proved to be a good cause as the manager from the customer side, sent a good mail to my manager to congratulate me for my efforts and going the extra mile to support the customer and the services. The product was a success after a couple of months as many subscribers and merchants took up the new technology that was NFC(Near Field Communication).

#### **Tell us about a time where you helped someone.**
One time during one of my leave days, my neighbour had a rebuild project for his house and needed to repaint the whole house. He was going to do all this by himself, but since I was free and on leave, I decided to help him and in the process learnt the different types of paints to use, when to use them and which paint is durable. In the process, the neighbour also shared more life lessons since he was elderly compare to me and some of the advice he gave me, I use them in my daily work.

#### **What appeals to you about GitHub, as a company you'd potentially be working for?**
GitHub supports a community where more than 50 million people learn, share, and work together to build software and collaborate and in the process automating from code to the cloud through the CI/CD feature which allows for a business to scale faster. To be a part of the team that ensures all customers and the Github community has a seamless and beautiful experience while using the awesome GitHub features is what I want to be a part of and help bring change to the world as well as be innovative in the process.
I am also an avid follower of GitHub social media pages like twitter and I love that the brand really engages with its customers and feels really connected to the people it serves.
Coupled with the necessary skills in GIT, Cloud technology, great customer support experiences, and passion I will be an incredible match with GitHub.

#### **How would you describe what GitHub does to a non-technical person?**
GitHub is a web-based site that allows you to store something that is written or a text file. GitHub lets people create new versions of the stored file, as well as have access to previous versions saved along the way after modifications done on the file. Everyone can access GitHub and share stuff with each other if they want as per the permissions set.

#### **What motivates you to work in support?**
I am passionate about putting a smile on the customers' face, and fixing any issues that the customers raise. Being the first contact with the customers ensures that I can create a rapport with the customer and ensure that they have a seamless experience using different applications and also explain to them whenever they need clarification. At the end of the day, a happy customer is good for the business and that fills me with joy to know that I made a customer happy by fixing or assisting them to resolve an issue they had.

