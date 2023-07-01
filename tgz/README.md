## tgz folder content

This folders contains tarballs with changes to test / install

### patchmanager-unified-pm_scripts-v0.0.8.tgz

I have unified the `pm_apply` and `pm_unapply` shells script in a single one `pm_patch.env` because most of the code was redundant.

* `pm_apply` does `source pm_patch.env apply "$@"`
* `pm_unapply` does `source pm_patch.env unapply "$@"`

This would help to maintain such shell script code in the future.
