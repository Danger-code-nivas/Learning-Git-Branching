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
<img width="1910" height="915" alt="Screenshot 2025-12-22 184642" src="https://github.com/user-attachments/assets/54d5d324-4e9c-4076-9b88-e21ddc213dd1" />
<h3>Level 2</h3>
<img width="1912" height="913" alt="Screenshot 2025-12-22 185617" src="https://github.com/user-attachments/assets/79643b75-1dfb-4655-9d33-1718238d87cd" />

<h2>Phase 4</h2>
<h3>Level 1</h3>
<img width="1904" height="907" alt="Screenshot 2025-12-22 190926" src="https://github.com/user-attachments/assets/572d1cbc-70c7-4261-8ecf-23d48f37c87b" />
<h3>Level 2</h3>
<img width="1900" height="908" alt="Screenshot 2025-12-22 213502" src="https://github.com/user-attachments/assets/12477447-f80a-47bb-aa90-77edf0519714" />
<h3>Level 3</h3>
<img width="1900" height="912" alt="Screenshot 2025-12-22 221001" src="https://github.com/user-attachments/assets/d46a978c-afc5-44bf-a421-1c6ad4844a45" />
<h3>Level 4</h3>
<img width="1902" height="908" alt="Screenshot 2025-12-22 221242" src="https://github.com/user-attachments/assets/9a7b115a-67c3-47fa-92ae-c4c5741210b2" />
<h3>Level 5</h3>
<img width="1901" height="905" alt="Screenshot 2025-12-22 221351" src="https://github.com/user-attachments/assets/01af4c8d-29b3-4300-b96b-0d382ebeb786" />

<h2>Phase 5</h2>
<h3>Level 1</h3>
<img width="1900" height="920" alt="Screenshot 2025-12-22 222036" src="https://github.com/user-attachments/assets/4aabbb71-7c1e-477a-9566-7231faacab92" />
<h3>Level 2</h3>
<img width="1895" height="902" alt="Screenshot 2025-12-22 222054" src="https://github.com/user-attachments/assets/0f869887-9460-4b23-921e-911c674caf91" />
<h3>Level 3</h3>
<img width="1893" height="910" alt="Screenshot 2025-12-22 222445" src="https://github.com/user-attachments/assets/287893a1-809f-4d90-802b-ebbf0a6a42fc" />
<h3>Level 4</h3>
<img width="1874" height="915" alt="Screenshot 2025-12-22 224706" src="https://github.com/user-attachments/assets/d3235e7c-76c5-49bf-b1ff-581f0f9265f2" />
<h3>Level 1</h3>
<img width="1906" height="912" alt="Screenshot 2025-12-22 224631" src="https://github.com/user-attachments/assets/f31536fa-0383-465f-bd75-f01f4839d93a" />
