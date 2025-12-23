<h1>Learning Git Branch</h1>
<p>Learning Git branches helps you manage different versions of your code without affecting the main project. It makes experimentation and collaboration easy by keeping changes organized and isolated</p>
<h2>Phase 1</h2>
<h3>Level 1</h3>
<h5>Introduced To Git Commits</h5>
<P>Learning Git branches helps you create separate paths to work on new ideas or fixes without affecting the main code. Getting introduced to Git commits teaches you how to save changes step by step, making teamwork and project tracking simple and clear.</P>
<img width="1917" height="854" alt="Screenshot 2025-12-23 122415" src="https://github.com/user-attachments/assets/1a8b6438-b241-4c9c-a7bd-d275066228ce" />

<h5>Code:</h5>

``` git commit ```

<img width="1908" height="909" alt="Screenshot 2025-12-22 143855" src="https://github.com/user-attachments/assets/ca44a7bf-1c10-4577-8bdf-2dae9ec8466c" />

<h3>Level 2</h3>
<h5>Branching in Git</h5>
<P>Branching in Git means creating a separate line of development where you can make changes without affecting the main project. It’s useful because it lets you experiment, fix bugs, or add new features safely before merging everything together.</P>
<img width="1919" height="850" alt="Screenshot 2025-12-23 230423" src="https://github.com/user-attachments/assets/602d1915-69f7-4ddd-99bd-9e37a091b7f6" />
<h5>Code:</h5>

```

git branch bugFix
git Checkout bugFix

```

<img width="1910" height="907" alt="Screenshot 2025-12-22 144146" src="https://github.com/user-attachments/assets/7aa73f08-40dc-4edf-a011-39cc64d3b5fc" />

<h3>Level 3</h3>
<h5>Merging in Git</h5>
<p>Merging in Git means combining changes from one branch into another to bring everyone’s work together. It’s useful because it lets teams integrate updates smoothly and keep the project code up to date.</p>
<img width="1919" height="854" alt="Screenshot 2025-12-23 231608" src="https://github.com/user-attachments/assets/6d33df24-8391-4421-8e60-cd94fe2fbd20" />

<h5>Code:</h5>

```
git branch bugFix
git checkout bugFix
git commit
git merge bugFix

```

<img width="1918" height="1012" alt="Screenshot 2025-12-22 145041" src="https://github.com/user-attachments/assets/7611ad1e-c066-4a28-80e0-d4722469fa38" />

<h3>Level 4</h3>
<h5>Rebasing in Git</h5>
<p>Rebasing in Git means moving or combining a series of commits onto a new base to create a cleaner project history. It’s useful because it keeps the commit timeline organized and makes collaboration easier to follow.</p>
<img width="1919" height="852" alt="Screenshot 2025-12-23 232113" src="https://github.com/user-attachments/assets/87414f1c-e00e-4b1c-a504-266975f3b42c" />

<h5>Code:</h5>

```

git branch bugFix
git checkout bugFix
git commit
git rebase main

```

<img width="1908" height="1010" alt="Screenshot 2025-12-22 145401" src="https://github.com/user-attachments/assets/37b9a0a0-fc98-473d-92d2-da733f8d0cb0" />

<h2>Phase 2</h2>
<h3>Level 1</h3>
<h5>Detach yo' HEAD</h5>
<p>In Git, “detached HEAD” means you’re viewing or working on a specific commit instead of a branch. It’s useful for testing or checking old versions of your project without changing your main branches.</p>
<img width="1919" height="850" alt="Screenshot 2025-12-23 232523" src="https://github.com/user-attachments/assets/f070fa6d-2641-4af1-a834-8c567bf49969" />

<h5>Code:</h5>

```

git checkout c4

```

<img width="1910" height="913" alt="Screenshot 2025-12-22 145704" src="https://github.com/user-attachments/assets/0fc9f744-937c-47c7-894f-2cc99d381e5c" />


<h3>Level 2</h3>
<h5>Relative Refs (^)</h5>
<p>Relative refs with the ^ symbol in Git let you refer to a commit’s parent, like HEAD^ for “one step before the current commit.” This is useful because it gives a quick way to move around your history without needing long commit IDs.</p>
<img width="1919" height="852" alt="Screenshot 2025-12-23 233832" src="https://github.com/user-attachments/assets/c5ac7780-732a-4814-9f03-5bca72bc9ede" />

<h5>Code:</h5>

```

git checkout HEAD^

```

<img width="1900" height="912" alt="Screenshot 2025-12-22 150016" src="https://github.com/user-attachments/assets/d9c3ba94-f337-440d-b496-db794c7e5143" />

<h3>Level 3</h3>
<h5>Relative Refs #2 (~)</h5>
<p>Relative refs with the ~ symbol in Git let you jump back several commits in a straight line, like HEAD~2 for “two commits before the current one.” This is useful because it gives a quick, readable way to explore or reference older points in your project history without copying long commit hashes.
</p>
<img width="1919" height="850" alt="Screenshot 2025-12-23 234346" src="https://github.com/user-attachments/assets/2506bf82-21d8-4436-876e-98a412c1fe4d" />

<h5>Code:</h5>

```

git branch -f main c6
git branch -f bugFix HEAD~2
git checkout c1
 
```

<img width="1919" height="910" alt="Screenshot 2025-12-22 151747" src="https://github.com/user-attachments/assets/aacc2865-cf9e-474c-8360-767f9d1d8699" />

<h3>Level 4</h3>
<h5>Reversing changes in Git</h5>
<p>Reversing changes in Git means undoing commits, stashes, or modifications to return your code to an earlier state without losing history. It's useful because it lets you fix mistakes, experiment safely, or clean up your project timeline easily.</p>
<img width="1919" height="851" alt="Screenshot 2025-12-23 235418" src="https://github.com/user-attachments/assets/ffc0fa84-91d2-412b-a980-d0a9916454d5" />

<h5>Code:</h5>

```

git branch -f local c1
git checkout pushed
git revert pushed

```

<img width="1908" height="913" alt="Screenshot 2025-12-22 152052" src="https://github.com/user-attachments/assets/f121b653-9d83-42af-9170-5e06fe1c2764" />


<h2>Phase 3</h2>
<h3>Level 1</h3>
<h5>Cherry-pick in Git</h5>
<p>Cherry-pick in Git means grabbing a specific commit from one branch and applying it exactly to another branch. It's useful because it lets you selectively move fixes or features without merging entire histories, keeping your project clean and targeted.</p>
<img width="1919" height="853" alt="Screenshot 2025-12-24 000134" src="https://github.com/user-attachments/assets/7e959b01-af86-4031-a278-6df64fc344bb" />

<h5>Code:</h5>

```

git cherry-pick c3 c4 c7

```
<img width="1902" height="952" alt="Screenshot 2025-12-22 152339" src="https://github.com/user-attachments/assets/a5f4c1f7-2552-42ff-ab4c-bdb031886dfd" />


<h3>Level 2</h3>
<h5>Interactive Rebase Intro</h5>
<p>Interactive rebase in Git means editing your commit history by reordering, squashing, or rewriting commits in an interactive session. It's useful because it cleans up messy histories, fixes errors, and makes your project timeline look professional before sharing with a team.</p>
<img width="1919" height="850" alt="Screenshot 2025-12-24 000511" src="https://github.com/user-attachments/assets/5e435952-b2d6-4c08-92ab-0e439e6be582" />

<h5>Commands used:</h5>

```

git rebase -i HEAD~4
git branch -f main c5
git branch -f overHere c5'
git chechout c5'
git checkout main
git rebase overHere


```
<img width="1910" height="915" alt="Screenshot 2025-12-22 184642" src="https://github.com/user-attachments/assets/47c273ba-ef72-407d-81bc-86be26484d64" />



<h2>Phase 4</h2>
<h3>Level 1</h3>
<h5>Grabbing Just 1 Commit</h5>
<p>Grabbing just 1 commit in Git means using cherry-pick to apply a single specific commit from anywhere to your current branch. It's useful because it lets you pull in one fix or feature without merging whole branches, keeping your changes precise and history clean.</p> 
<img width="1916" height="853" alt="Screenshot 2025-12-24 003204" src="https://github.com/user-attachments/assets/a59ef677-7a52-419c-a5c0-7b15ad7e5483" />

<h5>Commands used:</h5>

```

git rebase -i HEAD~3
git checkout main
git branch -f main c4'

```

<img width="1904" height="907" alt="Screenshot 2025-12-22 190926" src="https://github.com/user-attachments/assets/b6093856-ccb5-452b-9222-3bb551583bb3" />

<h3>Level 2</h3>
<h5>Juggling Commits</h5>
<p>Juggling commits in Git means using interactive rebase to reorder, combine, or split commits for a cleaner project history. It's useful because it helps tidy up your work, fix mistakes, and present a professional timeline when collaborating with others.</p>
<img width="1917" height="850" alt="Screenshot 2025-12-24 003646" src="https://github.com/user-attachments/assets/0675b010-9491-4946-84eb-4b77494e8c0e" />

<h5>Commands used:</h5>

```

git rebase -i HEAD~2
git checkout newImage
git rebase caption
git branch -f newImage c2
git branch -f caption c3
git checkout caption
git rebase -i HEAD~2
git checkout main
git branch -f main c3''


```

<img width="1900" height="908" alt="Screenshot 2025-12-22 213502" src="https://github.com/user-attachments/assets/40874791-2d74-45b4-a0e9-f6034d82fb19" />


<h3>Level 3</h3>
<h5>Juggling Commits #2</h5>
<p>Juggling commits #2 in Git means advancing your skills with interactive rebase to fix up, edit, or drop specific commits during a session. It's useful because it gives precise control over history tweaks, making your project narrative smoother and more shareable with teams.</p>
<img width="1917" height="852" alt="Screenshot 2025-12-24 003859" src="https://github.com/user-attachments/assets/d8b64661-8836-4184-bfd5-fe3740be9030" />

<h5>Commands used:</h5>

```

git checkout newImage
git checkout main
git cherry-pick c2
git branch -f main c1
git cherry-pick c2
git cherry-pick c3

```

<img width="1900" height="912" alt="Screenshot 2025-12-22 221001" src="https://github.com/user-attachments/assets/026b9e9e-ff40-4fef-b9b3-c0180116b05e" />

<h3>Level 4</h3>
<h5>Git Tags</h5>
<p>Git tags mark specific commits with a fixed label, like "v1.0" for a release version. They're useful because they create easy-to-remember snapshots of your code for quick reference, rollbacks, or sharing stable points with teams.</p>
<img width="1919" height="848" alt="Screenshot 2025-12-24 004117" src="https://github.com/user-attachments/assets/79dee88d-54cb-4630-9e5c-e66c356e9d3c" />

<h5>Commands used:</h5>

```

git tag v0 c1
git checkout c2
git tag v1 c2

```

<img width="1902" height="908" alt="Screenshot 2025-12-22 221242" src="https://github.com/user-attachments/assets/a7a8a6b3-9228-4f10-9381-1a78917f36e4" />

<h3>Level 5</h3>
<h5>Git Describe</h5>
<p>Git describe means finding the closest tag to a commit and labeling it with the tag name plus commit count and hash, like "v1.2-5-gabc123." It's useful because it creates human-readable version identifiers for builds, releases, or scripts without memorizing long hashes.</p>
<img width="1919" height="851" alt="Screenshot 2025-12-24 004249" src="https://github.com/user-attachments/assets/96c0e093-7cd2-4ab7-a3c6-90f0a9f29d9f" />

<h5>Commands used:</h5>

```

git commit

```

<img width="1901" height="905" alt="Screenshot 2025-12-22 221351" src="https://github.com/user-attachments/assets/61373d7a-a9ff-4922-90a3-304b30bc785e" />


<h2>Phase 5</h2>
<h3>Level 1</h3>
<h5>Rebasing over 9000 times</h5>
<p>Rebasing over 9000 times in Git means practicing interactive rebase extensively on large commit histories to master advanced editing like squashing thousands of changes. It's useful because it builds confidence in reshaping complex timelines cleanly, preparing you for real-world team projects with messy histories.</p>
<img width="1917" height="847" alt="Screenshot 2025-12-24 005744" src="https://github.com/user-attachments/assets/428a08d2-17b1-448c-8812-81265ca93caa" />

<h5>Commands used:</h5>

```

git checkout bugFix
git rebase main
git branch -f main c4
git checkout main
git rebase bugFix
git branch -f main c5
git branch -f bugFix c4'
git rebase bugFix
git branch -f main c6
git branch -f bugFix c5'
git rebase bugFix
git branch -f main c7
git branch -f bugFix c6'
git rebase bugFix

```

<img width="1900" height="920" alt="Screenshot 2025-12-22 222036" src="https://github.com/user-attachments/assets/29bd0508-3f14-499f-a4c3-c0be5cc0ee8b" />



<h3>Level 2</h3>
<h5>Multiple parents</h5>
<p>Multiple parents in Git means a commit (like a merge) has more than one parent commit, showing where branches combined. It's useful because it tracks exactly how histories merged, helping you understand project evolution and resolve conflicts clearly.</p>
<img width="1919" height="851" alt="Screenshot 2025-12-24 005851" src="https://github.com/user-attachments/assets/5b6bd420-71bb-47c1-8cff-899dbf422442" />

<h5>Commands used:</h5>

```

git checkout c2
git branch bugWork
git checkout main

```

<img width="1893" height="910" alt="Screenshot 2025-12-22 222445" src="https://github.com/user-attachments/assets/31c05ff0-c6cc-41c3-bf77-148cdc378a17" />


<h3>Level 3</h3>
<h5>Branch Spaghetti</h5>
<p>Branch spaghetti in Git means a tangled mess of overlapping branches and merges that make the history graph look like messy noodles. It's useful to recognize because it teaches you to clean it up with rebase or resets, keeping your project history readable and professional.</p>
<img width="1915" height="851" alt="Screenshot 2025-12-24 005941" src="https://github.com/user-attachments/assets/568eb45e-e1c6-4f85-aed7-bfdfc19662bd" />

<h5>Commands used:</h5>

```

git checkout three
git branch -f three c4
git rebase -i HEAD~3
git checkout main
git rebase -i HEAD~4
git checkout three
git rebase main
git branch -f three c2
git branch -f main c4'
git checkout main
git cherry-pick c3 c2
git branch -f main c3'
git branch -f two c4''
git rebase two
git branch -f main c2'
git branch -f two c3''
git rebase two
git branch -f main c5
git branch -f two c2''
git branch -f one c2'

```

<img width="1906" height="912" alt="Screenshot 2025-12-22 224631" src="https://github.com/user-attachments/assets/c45e5290-698a-4718-a202-74afec10ee48" />

