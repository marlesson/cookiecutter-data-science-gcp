Commands
========

The Makefile contains the central entry points for common tasks related to this project.

Syncing data to GCP
^^^^^^^^^^^^^^^^^^

* `make sync_data_to_gcs` will use `gsutil rsync` to sync files in `data/` up to `gs://{{ cookiecutter.gcs_bucket }}/{{ cookiecutter.repo_name }}/data/`.
* `make sync_data_from_gcs` will use `gsutil rsyc` to sync files from `gs://{{ cookiecutter.gcs_bucket }}/{{ cookiecutter.repo_name }}/data/` to `data/`.
