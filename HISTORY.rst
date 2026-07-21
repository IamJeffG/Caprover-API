=======
History
=======

0.1.25 (2026-07-21)
-------------------

* Use `create_and_update_app` from `deploy_one_click_app`.
  This attempts to avoid a rare race condition when `deploy_one_click_app()` calls
  `update_app` too quickly after `create_app`: `create_and_update_app` includes some sleeps.

0.1.24 (2024-12-16)
-------------------

* Fix & test update from novel kwargs (#12)
* update method lets you set httpAuth (#11)
* `update()` now handles persistent directories that use hostPath (#7)
* `gen_random_hex` works across whole one-click-app YAML (#6)
* Bugfix: `update()` should not change notExposeAsWebApp (#8)
* Enable SSL on base domain (#9)
* Allow optional override one-click repository path (#5)

0.1.0 (2021-06-11)
------------------

* First release on PyPI.
