# ml-template
This is a template repository. This is used to create new repos for working on machine learning models.

## How to use this ?
To create a new repository from this template, Use the "Use this template" button above.

<img src="https://github.com/clouda-inc/ml-template/assets/140997769/895fdefd-454c-4112-bd18-9e74b993e1f3"  width="60%" height="60%">

## DVC
### Add files to DVC
`dvc add <file or folder that you want to track>` then `dvc push` then `git add .` then
`git commit -am "dvc files added"`

If you make changes to any existing dvc files. Make sure to `dvc add` them again and `dvc push`. Then `git commit`
### Pull from DVC
`dvc pull` or `dvc pull <file or folder>`


## Location of saved files
The files are saved at https://drive.google.com/drive/folders/1NjL5FJSqj_GxUfEMtQZa6DjZl_c8eqpL drive folder. 
Each person can use their 30GB gsuite quota. If someones quota is reached. Some old files can be deleted or we can move everythign to S3.


## Scripts 
- `scripts/dvc-set-token.sh` is used to setup the dvc token after you have uploaded the `default.json` into the root directory of this repo.

- `scripts/colab-ssh-error-fix.sh` is used to fix the error shown below when trying to `git clone <repo>` using Google CoLab. 
```Cloning into 'wordpress-integration'...
Host key verification failed.
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
```

## What is initialized
DVC

default.json added to .gitignore

## Example
Check out `Complete example on vast.ai` in https://docs.google.com/document/d/1Xs2tZ5mWpSIrvHpD5DSB6322o5bWFUd9eadfAKRxgZw/

Check out `Complete example of using this template on Google Colab` in https://docs.google.com/document/d/1mtYs4QrGbGlUkyPl75Qiq0PHq5fsYY708C6jfQ4bmp8/edit

## TODO
Add MLflow central tracking server details

## References 
[DVC Use Case example](https://dvc.org/doc/use-cases/versioning-data-and-models/tutorial)

[DVC version controlling youtube video](https://www.youtube.com/watch?v=kLKBcPonMYw&t=7s)
