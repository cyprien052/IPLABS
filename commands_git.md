
## Resolved merge conflict: force pulled online notebook from elise and keep my local notebook

git add .
git commit -m "adding my part"
git pull
git checkout --theirs Lab3/notebook/03_object_tracking_2025_by_Elise.ipynb
git add Lab3/notebook/03_object_tracking_2025_by_Elise.ipynb
git commit -m "Resolved merge conflict: force pulled Elise's notebook from online and kept Cyprien's notebook"
git push

## keep your local version and ignore the online version during a conflict
git checkout --ours "path/to/file.ipynb"
git add "path/to/file.ipynb"
git commit -m "Kept local version of the notebook"
git push