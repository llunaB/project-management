### π commit convention

- `feat` : new feature for the user, not a new feature for build script
- `fix` : bug fix for the user, not a fix to a build script
- `docs` : changes to the documentation
- `style` : formatting, missing semi colons, etc; no production code change
- `refactor` : refactoring production code, eg. renaming a variable
- `chore` : updating grunt tasks etc; no production code change

```bash
feat: profile-history schrollbar add
```



### β­οΈ git flow 

##### 1. git clone

```bash
git clone https://lab.ssafy.com/s06-webmobile1-sub1/S06P11A206.git
```

##### 2. develop λΈλμΉλ‘ μ΄λ

```bash
git switch develop
```

 ### π  feature work flow

 ##### 3. feature branch μμ±

```bash
git branch feature/be/user/login
```
##### 4. feature branch λ‘ μ΄λ

```bash
git switch feature/be/user/login
```

##### 5. βΌοΈ**μ€μ**βΌοΈ develop branch pull μ§ν 

```bash
git pull origin develop
```

##### 6. κ°λ° ν add - commit - push μ§ν

- μΌλ°μ μΌλ‘λ `develop` λΈλμΉμ λ°λ‘ `push` νμ§λ§,  ssafy projectμμλ μ§νμ¬ν­ νμΈμ μν΄  `feature branch` λ `remote` μ μ¬λ¦½λλ€.

```bash
git add .
git commit -m "feat: profile-history schrollbar add"
git push origin develop
```

##### 7. feature branch μμ κ°λ° μ§ν

- `convention` μ°Έκ³ 
```bash
git add .
git commit -m "feat: profile-history schrollbar add"
git push origin feature/be/user/login
```

##### 8. νμ€νΈκΉμ§ μ§ν ν develop branchμ merge μ§ν
- `assignee` μ `reviewer`λ νμμ λ±λ‘ν©λλ€.

- λ°©λ² 1 : `feature branch` μμ `develop branch` λ‘ `push` 

```bash
# feature 
git push origin develop
```

- λ°©λ² 2 : `develop branch` μμ `feature branch` λ₯Ό `merge` 

```bash
# develop 
git merge feature/be/user/login
```

##### 9. merge request μμ±

- `gitlab` μ νΈμμλ¦Ό νμΈ
- `merge request` λ§λ€κΈ°
- λ΄μ© μλ ₯ ν `delete branch after merge request` μ²΄ν¬λμ΄μλμ§ νμΈ, βΌοΈ**μ²΄ν¬ ν΄μ **βΌοΈ
- `merge` 

##### 10. develop branch pull
- `pull` μ λ§€λ² ν΄μ£ΌκΈ°
```bash
git pull origin develop
```
