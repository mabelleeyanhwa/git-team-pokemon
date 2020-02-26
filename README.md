# Git Team with Pokemon

Practice using Git and Github as a team with Pokemon!

## 1. Merge Hell Simulation

In this exercise, we are all working in pairs, one 1 single repository on GitHub.

First, we shall add everyone as collaborators to a repository.

We need to form the best Pokemon teams to beat the Elite Four. We have to form three teams of six pokemons each Every pair is allowed to choose their own pokemon to be added to the team. Our job is to replace all the lorem ipsum words with your favourite pokemon.

We will pair up and make changes according to the instructions below, and experience merge hell
for ourselves!

### 1a. Merge conflicts on master branch

Only modify the files in `batch1` folder.

Each pair shall compete to add their favourite pokemon in `team1.txt`, `team2.txt` and `team3.txt`. You can only commit and push **once**. Replace the lorem ipsum lines with your favourite pokemon.

To qualify, your commit message needs to follow this convention: `[first person's name / second person's name] <commit message>`. For example: `[Elson/Jesstern] Add two pokemons to team1.txt`.

The pair with the most pokemon that are theirs wins! First pair to push also wins! ;)
The other pairs need to do `git pull --rebase`. Once you have resolved the merge conflict, do `git add` and `git rebase --continue`.

### 1b. Merge conflicts across branches

Only modify the files in `batch2` folder.

- Each pair shall create a local branch: `git checkout -b team1-feature`
- For each lorem ipsum line in each file, replace the lorem ipsum line with your favourite pokemon. Make a commit for each pokemon replacement.

Wait! Now the rules have changed. We can only send 4 pokemon to the Elite Four now!

team1.txt on the master branch shall now be changed to:

```
Team 1
1. lorem ipsum
2. lorem ipsum
3. lorem ipsum
4. lorem ipsum
```

- Checkout to master `git checkout master`
- Add and commit

Now for each pair:

- Ensure you are on master branch. `git checkout master`
- Do `git merge team1-feature` to merge your features from your local team1-feature branch onto your local master branch
- Push your changes to the remote master branch. Oh you can't push? There is a conflict! Do a `git pull` now.
- You will see merge conflicts, fix the merge conflicts and do a `git add ..`
- Using this method, we will create a merge commit. `git commit -m "..."` to complete the merge
- Push the changes to the remote master branch `git push` 

## 2. Pull Request

Only modify the files in `batch2` folder.

Calling all pokemon trainers! We need a lot more teams to join the Battle Tower!

Each pair shall now add a new team by adding a new txt file. 

- add a new txt file
- create a new pull request on Github 
- request a review from another pair
- the other pair should make some comments in the review. 
- the pair that created the PR can read the review and make the necessary changes before pushing again and updating the PR. 
- the other pair that reviewed can now merge the PR once they re-review the PR and approve it