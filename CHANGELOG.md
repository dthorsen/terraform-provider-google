## 0.1.0 (Unreleased)

BACKWARDS INCOMPATIBILITIES / NOTES:

* `compute_disk.image`: shorhand for disk images is no longer supported, and will display a diff if used [GH-1]

IMPROVEMENTS:

* Add an additional delay when checking for sql operations [GH-15170](https://github.com/hashicorp/terraform/pull/15170)
* Add support for importing `compute_backend_service` [GH-40]
* Wait for disk resizes to complete [GH-1]
* Support `connection_draining_timeout_sec` in `google_compute_region_backend_service` [GH-101]
* Add support for labels and tags on GKE node_config [GH-7]
* Made `path_rule` optional in `google_compute_url_map`'s `path_matcher` block [GH-118]

BUG FIXES:

* Changed `google_compute_instance_group_manager` `target_size` default to 0 [GH-65]
* Represent GCS Bucket locations as uppercase in state. [GH-117]
