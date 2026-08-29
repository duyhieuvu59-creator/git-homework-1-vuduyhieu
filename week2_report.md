Week2 Git Report

$ touch week2_report.md
$ git add week2_report.md
$ git commit -m "Submit week2_report.md"

* PART A:
$ git switch main
$ touch week2.md
$ git add week2.md
$ git commit -m "Create week2.md"
$ git switch -c week2
$ echo "working 1" >> week2.md
$ git add week2.md
$ git commit -m "working 1"
$ echo "working 2" >> week2.md
$ git add week2.md
$ git commit -m "working2"
$ echo "anything123..." >> week2.md
$ git add week2.md
$ git commit -m "Anything123..."
$ git switch main
$ echo "Khi chuyen ve master, cac noi dung them vao da bien mat vi chung chi ton tai tren nhanh week2" >> week2.md
$ git add week2.md
$ git commit -m "Document findings in week2.md"
$ git switch -c week2b
$ git merge week2 --no-ff -m "3-way merge week2 vao week2b"
$ git branch -d week2

* PART B:
$ git merge --abort
$ git switch -c wip
$ touch wip.txt
$ git add wip.txt
$ git commit -m "Create wip.txt"
$ git switch main
$ git merge week2b
$ echo "NHÁNH ĐÃ MERGE" >> week2.md
$ git branch --merged >> week2.md
$ echo "NHÁNH CHƯA MERGE" >> week2.md
$ git branch --no-merged >> week2.md
$ git add week2.md
$ git commit -m "Add branch filter commands output"
$ git branch -d week2b
$ git branch -m wip work-in-progress
$ git push -u origin work-in-progress

* PART C:
$ git switch work-in-progress
$ git branch -vv

* PART D:
$ git switch main
$ git switch -c experiment
$ touch exp1.txt
$ git add exp1.txt
$ git commit -m "Experiment commit 1"
$ touch exp2.txt
$ git add exp2.txt
$ git commit -m "Experiment commit 2"
$ git switch main
$ touch main_update.txt
$ git add main_update.txt
$ git commit -m "Cap nhat nhanh de tao su phan tach"
$ git switch experiment
$ git rebase master
$ git switch master
$ echo "Giải thích Rebase: Lệnh rebase đã nhấc các commit của nhánh 'experiment' ra và áp đặt lại nối tiếp lên trên commit mới nhất của nhánh 'master'. Việc này định tuyến lại lịch sử thành một đường thẳng duy nhất, tránh tạo ra commit gộp (merge commit) thừa thãi." >> week2.md
$ git add week2.md
$ git commit -m "Explain rebase in week2.md"
$ git merge experiment
$ git push origin master
$ git add week2_report.md
$ git commit -m "Add week2_report.md documenting all codes"
$ git push origin master
