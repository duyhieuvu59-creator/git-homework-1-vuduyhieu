On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	./

nothing added to commit but untracked files present (use "git add" to track)
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	new file:   notes.txt
	new file:   todo.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	draft.md
	status_log.md

diff --git a/part1/notes.txt b/part1/notes.txt
index e69de29..4fe7cd8 100644
--- a/part1/notes.txt
+++ b/part1/notes.txt
@@ -0,0 +1,3 @@
+abc
+asdfghjkl
+qwertyuiop
diff --git a/part1/notes.txt b/part1/notes.txt
index e69de29..4fe7cd8 100644
--- a/part1/notes.txt
+++ b/part1/notes.txt
@@ -0,0 +1,3 @@
+abc
+asdfghjkl
+qwertyuiop
### Tai sao 'git commit -a' chi hoat dong voi tracked files:
Co -a tu dong stage cac file da duoc theo doi, bi sua hoac xoa nhung bo qua cac file moi (untracked) vi Git yeu cau xac nhan bang 'git add' truoc.
### Su khac nhau giua git fetch va git pull:
- git fetch: Tai cac commit moi tu remote repo ve nhung KHONG tu dong gop (merge) vao code local. Cho phep kiem tra truoc khi gop.
- git pull: Tu dong thuc hien git fetch va ngay lap tuc gop (merge) cac thay doi tu remote vao branch local hien tai.
