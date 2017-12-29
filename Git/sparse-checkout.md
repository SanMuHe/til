# Sparse Checkout

If your remote Git repro is big and you only need to work on some particular files or sub-directories of the repro, you can use Git's sparse checkout feature to checkout only those particular files or sub-directories:

```bash
mkdir my_repo
cd my_repo
git init
git config core.sparseCheckout true
echo 'path/to/subdir1/' >> .git/info/sparse-checkout
echo 'path/to/subdir2/' >> .git/info/sparse-checkout
...
echo 'path/to/file1/' >> .git/info/sparse-checkout
echo 'path/to/file2/' >> .git/info/sparse-checkout
...
git remote add -f origin ssh://... (or https://...)
git pull origin master
```
