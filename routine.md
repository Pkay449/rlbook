To work on your `pk-main` branch while staying updated with the teacher's `main` branch (`upstream/main`), follow this **routine**:

---

### **Routine for Working on Your `pk-main` Branch**

---

#### **1. Start Your Session**

1. **Navigate to Your Repository:**
   ```bash
   cd ~/Github_NoCloud/rlbook
   ```

2. **Fetch Updates from `upstream`:**
   Always fetch the latest changes from the teacher's repository before you start working:
   ```bash
   git fetch upstream
   ```

3. **Merge Updates into Your `main` Branch:**
   Keep your `main` branch in sync with the teacher’s branch:
   ```bash
   git checkout main
   git merge upstream/main
   ```

4. **Push the Updated `main` Branch to Your Fork:**
   Reflect the updates in your fork’s `main` branch:
   ```bash
   git push origin main
   ```

---

#### **2. Bring Updates to Your `pk-main` Branch**

1. Switch to Your `pk-main` Branch:
   ```bash
   git checkout pk-main
   ```

2. Merge Updates from `main` Into `pk-main`:
   Incorporate the latest changes from the teacher’s `main` branch:
   ```bash
   git merge main
   ```

3. Resolve Conflicts (if any):
   - If there are conflicts, Git will mark them in your files.
   - Open the conflicting files, look for `<<<<<<`, `======`, and `>>>>>>` markers, and decide how to combine the changes.
   - After resolving, mark the files as resolved:
     ```bash
     git add <file-name>
     ```
   - Continue the merge:
     ```bash
     git commit
     ```

4. Push the Updated `pk-main` Branch to Your Fork:
   ```bash
   git push origin pk-main
   ```

---

#### **3. Work on Your Branch**

1. **Make Changes in `pk-main`:**
   Edit files and make improvements in your branch.

2. **Commit Your Changes:**
   Add and commit your changes:
   ```bash
   git add .
   git commit -m "Description of the changes"
   ```

3. **Push Your Changes to Your Fork:**
   ```bash
   git push origin pk-main
   ```

---

#### **4. Periodically Sync Updates**
Repeat the steps in **1** and **2** regularly to ensure your work stays up-to-date with the teacher’s repository.

---

### **Summary of Commands**

#### Before Working:
```bash
# Fetch updates from upstream
git fetch upstream

# Merge updates into main and push
git checkout main
git merge upstream/main
git push origin main

# Merge updates into pk-main
git checkout pk-main
git merge main
git push origin pk-main
```

#### During Work:
```bash
# Make changes and commit
git add .
git commit -m "Description of changes"

# Push your changes to pk-main
git push origin pk-main
```

---

### **Best Practices**

1. **Work in Small Commits:**
   - Commit your changes often to keep track of progress.

2. **Test After Syncing:**
   - Test your branch (`pk-main`) after merging updates from `main` to ensure everything works as expected.

3. **Communicate Conflicts:**
   - If you consistently encounter conflicts during merges, review your workflow to avoid overlapping changes with `upstream/main`.

---

Let me know if you'd like me to automate this routine or create scripts for you! 😊