# Git_education

# клонирую репозиторий на локальную машину (только вертка mster)
git clone git@github.com:aleksei-sokolov/devops-school-git.git
cd devops-school-git
# указываю имя пользователя и почту пользователя для данного репозитория
git config user.name "Evgenii-Zuev"
git config user.email Evgenii_Zuev@epam.com
# нахожу все ветки в удаленном репозитории и скачиваю их на локальную машину
git branch -r | grep -v '\->' | sed "s,\x1B\[[0-9;]*[a-zA-Z],,g" | while read remote; do git branch --track "${r>
git fetch --all
# клонирую форкнутый репозиторий
git clone git@github.com:Evgenii-Zuev/devops-school-git.git
# изменяю путь до удаленного репозитория на свой
git remote set-url origin git@github.com:Evgenii-Zuev/Git_education.git
# загружаю локальные данный в свой удаленной репозиторий
git push --all
git checkout master
git rebase bugfix
git rebase roadmap
git rebase new_feature
git show e6cf891
vi code.txt
git add code.txt
git rebase --continue
git show cbea03c
vi test_results.txt
git add test_results.txt
git rebase --continue
nano author.txt
git add author.txt
git commit -m "Add author"

