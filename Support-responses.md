# Support-tickets

### **Ticket 1: Rejected pull request from fork**
*To start, I have to say I LOVE GITHUB. You guys rock. I was at your 4th birthday party,
thanks for the cupcake and booze!
Anyway, here's my problem. I sent a pull request to technoweenie, and he rejected it because
my master branch is out of sync with his master. What can I do to fix this?
Help me supportocat, you're my only hope!
/.Steve
Hint: You'll want to address their question, and you could add an explanation of topic
branches as a better workflow.*

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


### **Ticket 2: Syncing internal server and GitHub?**
*Hi GitHub! My company has an internal Git server used for deployments, we use GitHub,
and I work on a local copy of the repository. For workflow purposes, how do I sync my
repository to GitHub and the internal Git server?
Thanks,
vmg
Hint: One common option is Git remotes. There are others!*

### **Ticket 2 response:**
      replace this with your response


### **Ticket 3: Unhappy about forking**
*JamesTK here, I have another question.
One of my dev collaborator forked my private repo without explicit permission to do so... is
that typical? I am surprised that the system did not notify me if it was okay to grant the fork
permission. Is there a way to setup permissions of this sort? Also, other than asking the
collaborator to delete the forked repo, can I actually delete it?
Thanks, jamestk
Notes:
You've checked the account in our admin view, he only has one personal repository
(jamestk/tribbles), which has one collaborator. Any documentation you may need is available
on help.github.com.*

### **Ticket 3 response:**
      replace this with your response

## **Love to know more about yourself**
*We'd also love if you could share more about yourself so the team can get to know you
better! If you could fill the following out that would be great:*

#### **Name?**
      replace this with your answer

#### **Location?**
      replace this with your answer

#### **What's an impressionable experience you've had with customer service/support, and why?**
      replace this with your answer

#### **Tell us about a time where you helped someone.**
      replace this with your answer

#### **What appeals to you about GitHub, as a company you'd potentially be working for?**
      replace this with your answer

#### **How would you describe what GitHub does to a non-technical person?**
      replace this with your answer

#### **What motivates you to work in support?**
      replace this with your answer
