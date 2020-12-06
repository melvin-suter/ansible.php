# Template Guide

There are some differences, if this is a wrapper-role for an appliance, or if it is a standalone role.

## Standalone

[X] Add your variables to `defaults` and `vars`. You can delete the ones in there, except `role_include_files`.
[X] Add your `files` & `templates` to the folders
[X] Update your `handlers`, you can delete the ones in there. Those are just examples.
[X] Update the `meta` file. The minimum required are `role_name` and `description`
[X] Delete the files in `tasks/shared`, and update the `tasks/main.yml` to not include these anymore
* Create your tasks files in a subfolder of `tasks`. Don't use the root-folder.
* Add your tasks files to the variable `role_include_files` in `vars/main.yml`
* Rename `tests/vars/99_uniqconsulting.ROLENAME.yml` and add all needed variables with examples
* Rename `tests/install_X_rolename.yml` and add the correct role inside
* Remove `files/README.md`, `templates/README.md`, `setup_1.sh` and `setup.sh`
* Replace this file with `README_TEMPLATE.md` and edit it as needed
