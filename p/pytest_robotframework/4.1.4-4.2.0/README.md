# Comparing `tmp/pytest_robotframework-4.1.4.tar.gz` & `tmp/pytest_robotframework-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_robotframework-4.1.4.tar", last modified: Sat May 18 06:25:39 2024, max compression
+gzip compressed data, was "pytest_robotframework-4.2.0.tar", last modified: Fri May 24 04:48:03 2024, max compression
```

## Comparing `pytest_robotframework-4.1.4.tar` & `pytest_robotframework-4.2.0.tar`

### file list

```diff
@@ -1,263 +1,277 @@
--rw-r--r--   0        0        0     1067 2024-05-18 06:25:24.260061 pytest_robotframework-4.1.4/LICENSE
--rw-r--r--   0        0        0    17497 2024-05-18 06:25:24.260061 pytest_robotframework-4.1.4/README.md
--rw-r--r--   0        0        0     8026 2024-05-18 06:25:39.067921 pytest_robotframework-4.1.4/pyproject.toml
--rw-r--r--   0        0        0    28462 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/pytest_robotframework/__init__.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/pytest_robotframework/_internal/__init__.py
--rw-r--r--   0        0        0      559 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/pytest_robotframework/_internal/cringe_globals.py
--rw-r--r--   0        0        0      921 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/pytest_robotframework/_internal/errors.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/pytest_robotframework/_internal/pytest/__init__.py
--rw-r--r--   0        0        0      230 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/pytest_robotframework/_internal/pytest/exception_getter.py
--rw-r--r--   0        0        0    24868 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/pytest_robotframework/_internal/pytest/plugin.py
--rw-r--r--   0        0        0     5008 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/pytest_robotframework/_internal/pytest/robot_file_support.py
--rw-r--r--   0        0        0     1181 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/pytest_robotframework/_internal/pytest/xdist_utils.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/pytest_robotframework/_internal/robot/__init__.py
--rw-r--r--   0        0        0     4528 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/pytest_robotframework/_internal/robot/library.py
--rw-r--r--   0        0        0    26358 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/pytest_robotframework/_internal/robot/listeners_and_suite_visitors.py
--rw-r--r--   0        0        0     9198 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/pytest_robotframework/_internal/robot/utils.py
--rw-r--r--   0        0        0     2045 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/pytest_robotframework/_internal/utils.py
--rw-r--r--   0        0        0     3240 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/pytest_robotframework/hooks.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/pytest_robotframework/py.typed
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/scripts/__init__.py
--rw-r--r--   0        0        0      177 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/scripts/clear_pycache.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/__init__.py
--rw-r--r--   0        0        0    13801 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/conftest.py
--rw-r--r--   0        0        0      230 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/__init__.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/__init__.py
--rw-r--r--   0        0        0      104 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_ansi.py
--rw-r--r--   0        0        0      186 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_as_keyword_args_and_kwargs.py
--rw-r--r--   0        0        0      296 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_as_keyword_context_manager_try_except.py
--rw-r--r--   0        0        0      105 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_assertion_fails.py
--rw-r--r--   0        0        0      105 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_assertion_fails_with_assertion_hook.py
--rw-r--r--   0        0        0      195 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_assertion_fails_with_description.py
--rw-r--r--   0        0        0      196 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_assertion_fails_with_fail_message_hide_assert.py
--rw-r--r--   0        0        0      175 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_assertion_pass_hook_multiple_tests.py
--rw-r--r--   0        0        0      105 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_assertion_passes.py
--rw-r--r--   0        0        0      435 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_assertion_passes_custom_messages.py
--rw-r--r--   0        0        0      253 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_assertion_passes_hide_assert.py
--rw-r--r--   0        0        0      359 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_assertion_passes_hide_asserts_context_manager.py
--rw-r--r--   0        0        0      292 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_assertion_passes_show_assert_when_no_assertions_in_robot_log.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_assertion_rewritten_in_conftest_when_assertion_hook_enabled/__init__.py
--rw-r--r--   0        0        0       80 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_assertion_rewritten_in_conftest_when_assertion_hook_enabled/conftest.py
--rw-r--r--   0        0        0       57 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_assertion_rewritten_in_conftest_when_assertion_hook_enabled/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_catch_errors_decorator/__init__.py
--rw-r--r--   0        0        0      536 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_catch_errors_decorator/conftest.py
--rw-r--r--   0        0        0       67 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_catch_errors_decorator/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/__init__.py
--rw-r--r--   0        0        0      678 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/conftest.py
--rw-r--r--   0        0        0       67 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/test_foo.py
--rw-r--r--   0        0        0      163 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_class_has_separate_suite.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_class_separate_files/__init__.py
--rw-r--r--   0        0        0      121 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_class_separate_files/test_suite1.py
--rw-r--r--   0        0        0      121 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_class_separate_files/test_suite2.py
--rw-r--r--   0        0        0      228 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_class_three_tests_one_fail.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_collect_only_nested_suites/asdf/__init__.py
--rw-r--r--   0        0        0       64 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_collect_only_nested_suites/asdf/test_bar.py
--rw-r--r--   0        0        0       64 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_collect_only_nested_suites/asdf/test_foo.py
--rw-r--r--   0        0        0        8 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/config/tox.ini
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/foo/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/tests/__init__.py
--rw-r--r--   0        0        0       57 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/tests/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_config_file_in_different_location/__init__.py
--rw-r--r--   0        0        0        8 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_config_file_in_different_location/asdf/tox.ini
--rw-r--r--   0        0        0       57 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_config_file_in_different_location/test_asdf.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_correct_items_collected_when_collect_only/__init__.py
--rw-r--r--   0        0        0       64 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_correct_items_collected_when_collect_only/test_bar.py
--rw-r--r--   0        0        0       64 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_correct_items_collected_when_collect_only/test_foo.py
--rw-r--r--   0        0        0       87 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_doesnt_run_when_collecting.py
--rw-r--r--   0        0        0      130 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_error_moment.py
--rw-r--r--   0        0        0      148 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_error_moment_and_second_test.py
--rw-r--r--   0        0        0      130 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_error_moment_exitonerror.py
--rw-r--r--   0        0        0      171 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_error_moment_exitonerror_multiple_tests.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_error_moment_setup/__init__.py
--rw-r--r--   0        0        0      142 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_error_moment_setup/conftest.py
--rw-r--r--   0        0        0      106 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_error_moment_setup/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_error_moment_teardown/__init__.py
--rw-r--r--   0        0        0      145 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_error_moment_teardown/conftest.py
--rw-r--r--   0        0        0      106 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_error_moment_teardown/test_foo.py
--rw-r--r--   0        0        0      163 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_fixture.py
--rw-r--r--   0        0        0      625 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_fixture_scope.py
--rw-r--r--   0        0        0      225 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_full_stack_keyword_context_manager.py
--rw-r--r--   0        0        0      152 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_full_stack_keyword_decorator.py
--rw-r--r--   0        0        0       82 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_invalid_fixture.py
--rw-r--r--   0        0        0      243 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_keyword_and_pytest_raises.py
--rw-r--r--   0        0        0      218 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_keyword_decorator_args.py
--rw-r--r--   0        0        0      554 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_doesnt_suppress.py
--rw-r--r--   0        0        0      542 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_raises_in_body_and_exit.py
--rw-r--r--   0        0        0      468 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_raises_in_exit.py
--rw-r--r--   0        0        0      171 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_keyword_decorator_custom_name_and_tags.py
--rw-r--r--   0        0        0      148 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_keyword_decorator_docstring.py
--rw-r--r--   0        0        0      178 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_keyword_decorator_docstring_on_next_line.py
--rw-r--r--   0        0        0      445 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_keyword_decorator_returns_context_manager_that_isnt_used.py
--rw-r--r--   0        0        0      275 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_keyword_decorator_try_except.py
--rw-r--r--   0        0        0       85 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_keyword_names.py
--rw-r--r--   0        0        0      273 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_keyword_raises.py
--rw-r--r--   0        0        0      166 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_keywordify_context_manager.py
--rw-r--r--   0        0        0      127 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_keywordify_function.py
--rw-r--r--   0        0        0      280 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_keywordify_keyword_inside_context_manager.py
--rw-r--r--   0        0        0      545 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_listener_calls_log_file/Listener.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.264061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_listener_calls_log_file/__init__.py
--rw-r--r--   0        0        0       64 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_listener_calls_log_file/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_listener_not_run_during_collection/__init__.py
--rw-r--r--   0        0        0      597 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_listener_not_run_during_collection/conftest.py
--rw-r--r--   0        0        0      105 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_listener_not_run_during_collection/test_foo.py
--rw-r--r--   0        0        0       77 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_module_docstring.py
--rw-r--r--   0        0        0       62 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_multiple_runs.py
--rw-r--r--   0        0        0      186 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_nested_class.py
--rw-r--r--   0        0        0      188 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_nested_keyword_that_fails.py
--rw-r--r--   0        0        0      107 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_nested_suites/suite1/suite2/test_asdf.py
--rw-r--r--   0        0        0      107 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_nested_suites/suite1/suite3/test_asdf2.py
--rw-r--r--   0        0        0      126 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_nested_suites/test_top_level.py
--rw-r--r--   0        0        0       63 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_no_tests_found_when_tests_exist.py
--rw-r--r--   0        0        0       92 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_one_test_fails.py
--rw-r--r--   0        0        0       73 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_one_test_passes.py
--rw-r--r--   0        0        0      162 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_one_test_skipped.py
--rw-r--r--   0        0        0      100 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_parameterized_tags.py
--rw-r--r--   0        0        0      207 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_parametrize.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/a/__init__.py
--rw-r--r--   0        0        0      185 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/a/test_c.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/b/__init__.py
--rw-r--r--   0        0        0       72 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/b/conftest.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_pytest_runtest_protocol_item_hook/foo/__init__.py
--rw-r--r--   0        0        0      398 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_pytest_runtest_protocol_item_hook/foo/conftest.py
--rw-r--r--   0        0        0       67 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_pytest_runtest_protocol_item_hook/foo/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_pytest_runtest_protocol_session_hook/__init__.py
--rw-r--r--   0        0        0      471 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_pytest_runtest_protocol_session_hook/conftest.py
--rw-r--r--   0        0        0       67 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_pytest_runtest_protocol_session_hook/test_foo.py
--rw-r--r--   0        0        0      296 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_python_file_doesnt_get_parsed_as_robot_file.py
--rw-r--r--   0        0        0       64 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_args.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_keyword_in_python_test/__init__.py
--rw-r--r--   0        0        0       34 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_keyword_in_python_test/bar/bar.resource
--rw-r--r--   0        0        0      262 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_keyword_in_python_test/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_modify_args_hook/__init__.py
--rw-r--r--   0        0        0      119 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_modify_args_hook/conftest.py
--rw-r--r--   0        0        0      222 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_modify_args_hook/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_modify_args_hook_collect_only/__init__.py
--rw-r--r--   0        0        0      175 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_modify_args_hook_collect_only/conftest.py
--rw-r--r--   0        0        0      221 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_modify_args_hook_collect_only/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_modify_options_hook/__init__.py
--rw-r--r--   0        0        0      235 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_modify_options_hook/conftest.py
--rw-r--r--   0        0        0      222 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_modify_options_hook/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/__init__.py
--rw-r--r--   0        0        0      630 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/conftest.py
--rw-r--r--   0        0        0       62 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/test_foo.py
--rw-r--r--   0        0        0      498 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_options_merge_listeners/Listener.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_options_merge_listeners/__init__.py
--rw-r--r--   0        0        0      322 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_options_merge_listeners/test_foo.py
--rw-r--r--   0        0        0       64 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_options_variable.py
--rw-r--r--   0        0        0      498 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_options_variable_merge_listeners/Listener.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_options_variable_merge_listeners/__init__.py
--rw-r--r--   0        0        0      322 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_options_variable_merge_listeners/test_foo.py
--rw-r--r--   0        0        0      236 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_set_log_level.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_setup_fails/__init__.py
--rw-r--r--   0        0        0       90 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_setup_fails/conftest.py
--rw-r--r--   0        0        0       73 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_setup_fails/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_setup_passes/__init__.py
--rw-r--r--   0        0        0      116 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_setup_passes/conftest.py
--rw-r--r--   0        0        0      116 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_setup_passes/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_setup_skipped/__init__.py
--rw-r--r--   0        0        0      101 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_setup_skipped/conftest.py
--rw-r--r--   0        0        0       73 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_setup_skipped/test_foo.py
--rw-r--r--   0        0        0      305 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_suite_variables.py
--rw-r--r--   0        0        0      313 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_suite_variables_with_slash.py
--rw-r--r--   0        0        0      107 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_suites/suite1/test_asdf.py
--rw-r--r--   0        0        0       94 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_tags.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_teardown_fails/__init__.py
--rw-r--r--   0        0        0       93 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_teardown_fails/conftest.py
--rw-r--r--   0        0        0       73 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_teardown_fails/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_teardown_passes/__init__.py
--rw-r--r--   0        0        0      119 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_teardown_passes/conftest.py
--rw-r--r--   0        0        0      115 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_teardown_passes/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_teardown_skipped/__init__.py
--rw-r--r--   0        0        0      104 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_teardown_skipped/conftest.py
--rw-r--r--   0        0        0       73 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_teardown_skipped/test_foo.py
--rw-r--r--   0        0        0       78 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_test_case_docstring.py
--rw-r--r--   0        0        0       80 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_trace_ricing.py
--rw-r--r--   0        0        0      106 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_traceback.py
--rw-r--r--   0        0        0      108 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_two_tests_one_fail_one_pass.py
--rw-r--r--   0        0        0       77 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_two_tests_specified_by_full_path.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_two_tests_specified_by_full_path_in_different_files/__init__.py
--rw-r--r--   0        0        0       62 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_two_tests_specified_by_full_path_in_different_files/test_bar.py
--rw-r--r--   0        0        0       62 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_two_tests_specified_by_full_path_in_different_files/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_two_tests_two_files_one_fail_one_pass/__init__.py
--rw-r--r--   0        0        0       64 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_two_tests_two_files_one_fail_one_pass/test_one.py
--rw-r--r--   0        0        0       83 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_two_tests_two_files_one_fail_one_pass/test_two.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_two_tests_with_same_name_one_fail_one_pass/__init__.py
--rw-r--r--   0        0        0       63 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_two_tests_with_same_name_one_fail_one_pass/test_one.py
--rw-r--r--   0        0        0       82 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_two_tests_with_same_name_one_fail_one_pass/test_two.py
--rw-r--r--   0        0        0      121 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_unittest_class.py
--rw-r--r--   0        0        0      311 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_variables_list.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_variables_not_in_scope_in_other_suites/__init__.py
--rw-r--r--   0        0        0      303 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_variables_not_in_scope_in_other_suites/test_one.py
--rw-r--r--   0        0        0      222 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_variables_not_in_scope_in_other_suites/test_two.py
--rw-r--r--   0        0        0       57 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_xdist_n_0.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_xfail_fails/__init__.py
--rw-r--r--   0        0        0      133 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_xfail_fails/test_foo.py
--rw-r--r--   0        0        0       28 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_xfail_fails/tox.ini
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_xfail_fails_no_reason/__init__.py
--rw-r--r--   0        0        0      118 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_xfail_fails_no_reason/test_foo.py
--rw-r--r--   0        0        0       28 2024-05-18 06:25:24.268061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_xfail_fails_no_reason/tox.ini
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_xfail_passes/__init__.py
--rw-r--r--   0        0        0      123 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_xfail_passes/test_foo.py
--rw-r--r--   0        0        0       28 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_xfail_passes/tox.ini
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_xfail_passes_no_reason/__init__.py
--rw-r--r--   0        0        0      107 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_xfail_passes_no_reason/test_foo.py
--rw-r--r--   0        0        0       28 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_python/test_xfail_passes_no_reason/tox.ini
--rw-r--r--   0        0        0       32 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_collect_only_nested_suites/bar.robot
--rw-r--r--   0        0        0       32 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_collect_only_nested_suites/foo.robot
--rw-r--r--   0        0        0       32 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_correct_items_collected_when_collect_only/bar.robot
--rw-r--r--   0        0        0       32 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_correct_items_collected_when_collect_only/foo.robot
--rw-r--r--   0        0        0       36 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_doesnt_run_tests_outside_path/bar/asdf.robot
--rw-r--r--   0        0        0       36 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_doesnt_run_tests_outside_path/foo/asdf.robot
--rw-r--r--   0        0        0       44 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_doesnt_run_when_collecting.robot
--rw-r--r--   0        0        0       99 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_fails_when_import_error_and_exit_on_error.robot
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_init_file/__init__.py
--rw-r--r--   0        0        0       40 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_init_file/foo.robot
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_init_file_nested/__init__.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_init_file_nested/foo/__init__.py
--rw-r--r--   0        0        0       40 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_init_file_nested/foo/bar.robot
--rw-r--r--   0        0        0       40 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_init_file_nested/foo/foo.robot
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_keyword_decorator/__init__.py
--rw-r--r--   0        0        0       71 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_keyword_decorator/bar.robot
--rw-r--r--   0        0        0      151 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_keyword_decorator/foo.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_keyword_decorator_and_other_decorator/__init__.py
--rw-r--r--   0        0        0       71 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_keyword_decorator_and_other_decorator/bar.robot
--rw-r--r--   0        0        0      468 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_keyword_decorator_and_other_decorator/foo.py
--rw-r--r--   0        0        0      162 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_keyword_with_conflicting_name.robot
--rw-r--r--   0        0        0       62 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_line_number.robot
--rw-r--r--   0        0        0      535 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_listener_calls_log_file/Listener.py
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_listener_calls_log_file/__init__.py
--rw-r--r--   0        0        0       40 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_listener_calls_log_file/foo.robot
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_nested_keyword_that_fails/__init__.py
--rw-r--r--   0        0        0       71 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_nested_keyword_that_fails/bar.robot
--rw-r--r--   0        0        0      160 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_nested_keyword_that_fails/foo.py
--rw-r--r--   0        0        0       40 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_no_tests_found_when_tests_exist.robot
--rw-r--r--   0        0        0       32 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_one_test_fails.robot
--rw-r--r--   0        0        0       36 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_one_test_passes.robot
--rw-r--r--   0        0        0       32 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_one_test_skipped.robot
--rw-r--r--   0        0        0       61 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_parameterized_tags/foo.robot
--rw-r--r--   0        0        0       34 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_parameterized_tags/tox.ini
--rw-r--r--   0        0        0       95 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_run_keyword_and_ignore_error.robot
--rw-r--r--   0        0        0      115 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_setup_fails.robot
--rw-r--r--   0        0        0      111 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_setup_passes.robot
--rw-r--r--   0        0        0      107 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_setup_skipped.robot
--rw-r--r--   0        0        0      163 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_setup_with_args.robot
--rw-r--r--   0        0        0       96 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_tags.robot
--rw-r--r--   0        0        0      100 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_tags_in_settings.robot
--rw-r--r--   0        0        0        0 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_tags_with_kwargs/__init__.py
--rw-r--r--   0        0        0      722 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_tags_with_kwargs/conftest.py
--rw-r--r--   0        0        0       93 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_tags_with_kwargs/test_tags_with_kwargs.robot
--rw-r--r--   0        0        0      119 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_teardown_fails.robot
--rw-r--r--   0        0        0      115 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_teardown_passes.robot
--rw-r--r--   0        0        0      111 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_teardown_skipped.robot
--rw-r--r--   0        0        0       36 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_two_files_run_one_test/bar.robot
--rw-r--r--   0        0        0       54 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_two_files_run_one_test/foo.robot
--rw-r--r--   0        0        0       54 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_two_files_run_test_from_second_suite/asdf/foo.robot
--rw-r--r--   0        0        0       36 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_two_files_run_test_from_second_suite/fdsa/bar.robot
--rw-r--r--   0        0        0       55 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_two_tests_one_fail_one_pass.robot
--rw-r--r--   0        0        0       57 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_warning_on_unknown_tag.robot
--rw-r--r--   0        0        0      874 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/test_common.py
--rw-r--r--   0        0        0    32672 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/test_python.py
--rw-r--r--   0        0        0    10564 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/test_robot.py
--rw-r--r--   0        0        0     1286 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/test_robot_utils.py
--rw-r--r--   0        0        0     1776 2024-05-18 06:25:24.272061 pytest_robotframework-4.1.4/tests/type_tests.py
--rw-r--r--   0        0        0    18040 1970-01-01 00:00:00.000000 pytest_robotframework-4.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-24 04:47:50.211513 pytest_robotframework-4.2.0/LICENSE
+-rw-r--r--   0        0        0    17559 2024-05-24 04:47:50.211513 pytest_robotframework-4.2.0/README.md
+-rw-r--r--   0        0        0     8026 2024-05-24 04:48:03.739571 pytest_robotframework-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0    28462 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/__init__.py
+-rw-r--r--   0        0        0      559 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/cringe_globals.py
+-rw-r--r--   0        0        0      921 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/errors.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/pytest/__init__.py
+-rw-r--r--   0        0        0      230 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/pytest/exception_getter.py
+-rw-r--r--   0        0        0    26433 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/pytest/plugin.py
+-rw-r--r--   0        0        0     7021 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/pytest/robot_file_support.py
+-rw-r--r--   0        0        0     1181 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/pytest/xdist_utils.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/robot/__init__.py
+-rw-r--r--   0        0        0     4528 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/robot/library.py
+-rw-r--r--   0        0        0    26358 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/robot/listeners_and_suite_visitors.py
+-rw-r--r--   0        0        0     9785 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/robot/utils.py
+-rw-r--r--   0        0        0     2045 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/utils.py
+-rw-r--r--   0        0        0     3240 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/hooks.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/py.typed
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/scripts/__init__.py
+-rw-r--r--   0        0        0      177 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/scripts/clear_pycache.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/__init__.py
+-rw-r--r--   0        0        0    13801 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      230 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_common/test_no_tests_found_no_files/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_common/test_robot_file_and_python_file/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_common/test_robot_file_and_python_file/foo.robot
+-rw-r--r--   0        0        0       57 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_common/test_robot_file_and_python_file/test_bar.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/__init__.py
+-rw-r--r--   0        0        0      104 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_ansi.py
+-rw-r--r--   0        0        0      186 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_as_keyword_args_and_kwargs.py
+-rw-r--r--   0        0        0      296 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_as_keyword_context_manager_try_except.py
+-rw-r--r--   0        0        0      105 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_fails.py
+-rw-r--r--   0        0        0      105 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_fails_with_assertion_hook.py
+-rw-r--r--   0        0        0      195 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_fails_with_description.py
+-rw-r--r--   0        0        0      196 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_fails_with_fail_message_hide_assert.py
+-rw-r--r--   0        0        0      175 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_pass_hook_multiple_tests.py
+-rw-r--r--   0        0        0      105 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_passes.py
+-rw-r--r--   0        0        0      435 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_passes_custom_messages.py
+-rw-r--r--   0        0        0      253 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_passes_hide_assert.py
+-rw-r--r--   0        0        0      359 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_passes_hide_asserts_context_manager.py
+-rw-r--r--   0        0        0      292 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_passes_show_assert_when_no_assertions_in_robot_log.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_rewritten_in_conftest_when_assertion_hook_enabled/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_rewritten_in_conftest_when_assertion_hook_enabled/conftest.py
+-rw-r--r--   0        0        0       57 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_rewritten_in_conftest_when_assertion_hook_enabled/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_catch_errors_decorator/__init__.py
+-rw-r--r--   0        0        0      536 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_catch_errors_decorator/conftest.py
+-rw-r--r--   0        0        0       67 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_catch_errors_decorator/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/__init__.py
+-rw-r--r--   0        0        0      678 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/conftest.py
+-rw-r--r--   0        0        0       67 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/test_foo.py
+-rw-r--r--   0        0        0      163 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_class_has_separate_suite.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_class_separate_files/__init__.py
+-rw-r--r--   0        0        0      121 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_class_separate_files/test_suite1.py
+-rw-r--r--   0        0        0      121 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_class_separate_files/test_suite2.py
+-rw-r--r--   0        0        0      228 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_class_three_tests_one_fail.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_collect_only_nested_suites/asdf/__init__.py
+-rw-r--r--   0        0        0       64 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_collect_only_nested_suites/asdf/test_bar.py
+-rw-r--r--   0        0        0       64 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_collect_only_nested_suites/asdf/test_foo.py
+-rw-r--r--   0        0        0        8 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/config/tox.ini
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/foo/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/tests/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/tests/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_config_file_in_different_location/__init__.py
+-rw-r--r--   0        0        0        8 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_config_file_in_different_location/asdf/tox.ini
+-rw-r--r--   0        0        0       57 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_config_file_in_different_location/test_asdf.py
+-rw-r--r--   0        0        0      254 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_console_output.py
+-rw-r--r--   0        0        0       66 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_console_summary.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_correct_items_collected_when_collect_only/__init__.py
+-rw-r--r--   0        0        0       64 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_correct_items_collected_when_collect_only/test_bar.py
+-rw-r--r--   0        0        0       64 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_correct_items_collected_when_collect_only/test_foo.py
+-rw-r--r--   0        0        0       87 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_doesnt_run_when_collecting.py
+-rw-r--r--   0        0        0      130 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_error_moment.py
+-rw-r--r--   0        0        0      148 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_error_moment_and_second_test.py
+-rw-r--r--   0        0        0      130 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_error_moment_exitonerror.py
+-rw-r--r--   0        0        0      171 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_error_moment_exitonerror_multiple_tests.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_error_moment_setup/__init__.py
+-rw-r--r--   0        0        0      142 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_error_moment_setup/conftest.py
+-rw-r--r--   0        0        0      106 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_error_moment_setup/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_error_moment_teardown/__init__.py
+-rw-r--r--   0        0        0      145 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_error_moment_teardown/conftest.py
+-rw-r--r--   0        0        0      106 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_error_moment_teardown/test_foo.py
+-rw-r--r--   0        0        0      163 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_fixture.py
+-rw-r--r--   0        0        0      625 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_fixture_scope.py
+-rw-r--r--   0        0        0      225 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_full_stack_keyword_context_manager.py
+-rw-r--r--   0        0        0      152 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_full_stack_keyword_decorator.py
+-rw-r--r--   0        0        0       82 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_invalid_fixture.py
+-rw-r--r--   0        0        0      243 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_and_pytest_raises.py
+-rw-r--r--   0        0        0      218 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_args.py
+-rw-r--r--   0        0        0      554 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_doesnt_suppress.py
+-rw-r--r--   0        0        0      542 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_raises_in_body_and_exit.py
+-rw-r--r--   0        0        0      468 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_raises_in_exit.py
+-rw-r--r--   0        0        0      171 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_custom_name_and_tags.py
+-rw-r--r--   0        0        0      148 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_docstring.py
+-rw-r--r--   0        0        0      178 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_docstring_on_next_line.py
+-rw-r--r--   0        0        0      445 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_returns_context_manager_that_isnt_used.py
+-rw-r--r--   0        0        0      275 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_try_except.py
+-rw-r--r--   0        0        0       85 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_names.py
+-rw-r--r--   0        0        0      273 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_raises.py
+-rw-r--r--   0        0        0      166 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keywordify_context_manager.py
+-rw-r--r--   0        0        0      127 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keywordify_function.py
+-rw-r--r--   0        0        0      280 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keywordify_keyword_inside_context_manager.py
+-rw-r--r--   0        0        0      545 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_listener_calls_log_file/Listener.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_listener_calls_log_file/__init__.py
+-rw-r--r--   0        0        0       64 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_listener_calls_log_file/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_listener_not_run_during_collection/__init__.py
+-rw-r--r--   0        0        0      597 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_listener_not_run_during_collection/conftest.py
+-rw-r--r--   0        0        0      105 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_listener_not_run_during_collection/test_foo.py
+-rw-r--r--   0        0        0       77 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_module_docstring.py
+-rw-r--r--   0        0        0       62 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_multiple_runs.py
+-rw-r--r--   0        0        0      186 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_nested_class.py
+-rw-r--r--   0        0        0      188 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_nested_keyword_that_fails.py
+-rw-r--r--   0        0        0      107 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_nested_suites/suite1/suite2/test_asdf.py
+-rw-r--r--   0        0        0      107 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_nested_suites/suite1/suite3/test_asdf2.py
+-rw-r--r--   0        0        0      126 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_nested_suites/test_top_level.py
+-rw-r--r--   0        0        0       63 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_no_tests_found_when_tests_exist.py
+-rw-r--r--   0        0        0       92 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_one_test_fails.py
+-rw-r--r--   0        0        0       73 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_one_test_passes.py
+-rw-r--r--   0        0        0      162 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_one_test_skipped.py
+-rw-r--r--   0        0        0      100 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_parameterized_tags.py
+-rw-r--r--   0        0        0      207 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_parametrize.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/a/__init__.py
+-rw-r--r--   0        0        0      185 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/a/test_c.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/b/__init__.py
+-rw-r--r--   0        0        0       72 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/b/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_pytest_runtest_protocol_item_hook/foo/__init__.py
+-rw-r--r--   0        0        0      398 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_pytest_runtest_protocol_item_hook/foo/conftest.py
+-rw-r--r--   0        0        0       67 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_pytest_runtest_protocol_item_hook/foo/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_pytest_runtest_protocol_session_hook/__init__.py
+-rw-r--r--   0        0        0      471 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_pytest_runtest_protocol_session_hook/conftest.py
+-rw-r--r--   0        0        0       67 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_pytest_runtest_protocol_session_hook/test_foo.py
+-rw-r--r--   0        0        0      296 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_python_file_doesnt_get_parsed_as_robot_file.py
+-rw-r--r--   0        0        0       64 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_args.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_keyword_in_python_test/__init__.py
+-rw-r--r--   0        0        0       34 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_keyword_in_python_test/bar/bar.resource
+-rw-r--r--   0        0        0      262 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_keyword_in_python_test/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_args_hook/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_args_hook/conftest.py
+-rw-r--r--   0        0        0      222 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_args_hook/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_args_hook_collect_only/__init__.py
+-rw-r--r--   0        0        0      175 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_args_hook_collect_only/conftest.py
+-rw-r--r--   0        0        0      221 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_args_hook_collect_only/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_options_hook/__init__.py
+-rw-r--r--   0        0        0      235 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_options_hook/conftest.py
+-rw-r--r--   0        0        0      222 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_options_hook/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/__init__.py
+-rw-r--r--   0        0        0      630 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/conftest.py
+-rw-r--r--   0        0        0       62 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/test_foo.py
+-rw-r--r--   0        0        0      498 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_options_merge_listeners/Listener.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_options_merge_listeners/__init__.py
+-rw-r--r--   0        0        0      322 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_options_merge_listeners/test_foo.py
+-rw-r--r--   0        0        0       64 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_options_variable.py
+-rw-r--r--   0        0        0      498 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_options_variable_merge_listeners/Listener.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_options_variable_merge_listeners/__init__.py
+-rw-r--r--   0        0        0      322 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_options_variable_merge_listeners/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_run_two_files/__init__.py
+-rw-r--r--   0        0        0       55 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_run_two_files/test_a.py
+-rw-r--r--   0        0        0       55 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_run_two_files/test_b.py
+-rw-r--r--   0        0        0      236 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_set_log_level.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_setup_fails/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_setup_fails/conftest.py
+-rw-r--r--   0        0        0       73 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_setup_fails/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_setup_passes/__init__.py
+-rw-r--r--   0        0        0      116 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_setup_passes/conftest.py
+-rw-r--r--   0        0        0      116 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_setup_passes/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_setup_skipped/__init__.py
+-rw-r--r--   0        0        0      101 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_setup_skipped/conftest.py
+-rw-r--r--   0        0        0       73 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_setup_skipped/test_foo.py
+-rw-r--r--   0        0        0      305 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_suite_variables.py
+-rw-r--r--   0        0        0      313 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_suite_variables_with_slash.py
+-rw-r--r--   0        0        0      107 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_suites/suite1/test_asdf.py
+-rw-r--r--   0        0        0       94 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_tags.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_teardown_fails/__init__.py
+-rw-r--r--   0        0        0       93 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_teardown_fails/conftest.py
+-rw-r--r--   0        0        0       73 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_teardown_fails/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_teardown_passes/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_teardown_passes/conftest.py
+-rw-r--r--   0        0        0      115 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_teardown_passes/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_teardown_skipped/__init__.py
+-rw-r--r--   0        0        0      104 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_teardown_skipped/conftest.py
+-rw-r--r--   0        0        0       73 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_teardown_skipped/test_foo.py
+-rw-r--r--   0        0        0       78 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_test_case_docstring.py
+-rw-r--r--   0        0        0       80 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_trace_ricing.py
+-rw-r--r--   0        0        0      106 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_traceback.py
+-rw-r--r--   0        0        0      108 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_one_fail_one_pass.py
+-rw-r--r--   0        0        0       77 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_specified_by_full_path.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_specified_by_full_path_in_different_files/__init__.py
+-rw-r--r--   0        0        0       62 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_specified_by_full_path_in_different_files/test_bar.py
+-rw-r--r--   0        0        0       62 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_specified_by_full_path_in_different_files/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_two_files_one_fail_one_pass/__init__.py
+-rw-r--r--   0        0        0       64 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_two_files_one_fail_one_pass/test_one.py
+-rw-r--r--   0        0        0       83 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_two_files_one_fail_one_pass/test_two.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_with_same_name_one_fail_one_pass/__init__.py
+-rw-r--r--   0        0        0       63 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_with_same_name_one_fail_one_pass/test_one.py
+-rw-r--r--   0        0        0       82 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_with_same_name_one_fail_one_pass/test_two.py
+-rw-r--r--   0        0        0      121 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_unittest_class.py
+-rw-r--r--   0        0        0      311 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_variables_list.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_variables_not_in_scope_in_other_suites/__init__.py
+-rw-r--r--   0        0        0      303 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_variables_not_in_scope_in_other_suites/test_one.py
+-rw-r--r--   0        0        0      222 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_variables_not_in_scope_in_other_suites/test_two.py
+-rw-r--r--   0        0        0       57 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xdist_n_0.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_fails/__init__.py
+-rw-r--r--   0        0        0      133 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_fails/test_foo.py
+-rw-r--r--   0        0        0       28 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_fails/tox.ini
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_fails_no_reason/__init__.py
+-rw-r--r--   0        0        0      118 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_fails_no_reason/test_foo.py
+-rw-r--r--   0        0        0       28 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_fails_no_reason/tox.ini
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_passes/__init__.py
+-rw-r--r--   0        0        0      123 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_passes/test_foo.py
+-rw-r--r--   0        0        0       28 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_passes/tox.ini
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_passes_no_reason/__init__.py
+-rw-r--r--   0        0        0      107 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_passes_no_reason/test_foo.py
+-rw-r--r--   0        0        0       28 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_passes_no_reason/tox.ini
+-rw-r--r--   0        0        0       32 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_collect_only_nested_suites/bar.robot
+-rw-r--r--   0        0        0       32 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_collect_only_nested_suites/foo.robot
+-rw-r--r--   0        0        0       32 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_correct_items_collected_when_collect_only/bar.robot
+-rw-r--r--   0        0        0       32 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_correct_items_collected_when_collect_only/foo.robot
+-rw-r--r--   0        0        0       36 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_doesnt_run_tests_outside_path/bar/asdf.robot
+-rw-r--r--   0        0        0       36 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_doesnt_run_tests_outside_path/foo/asdf.robot
+-rw-r--r--   0        0        0       44 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_doesnt_run_when_collecting.robot
+-rw-r--r--   0        0        0       99 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_fails_when_import_error_and_exit_on_error.robot
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_init_file/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_init_file/foo.robot
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_init_file_nested/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_init_file_nested/foo/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_init_file_nested/foo/bar.robot
+-rw-r--r--   0        0        0       40 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_init_file_nested/foo/foo.robot
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_keyword_decorator/__init__.py
+-rw-r--r--   0        0        0       71 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_keyword_decorator/bar.robot
+-rw-r--r--   0        0        0      151 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_keyword_decorator/foo.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_keyword_decorator_and_other_decorator/__init__.py
+-rw-r--r--   0        0        0       71 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_keyword_decorator_and_other_decorator/bar.robot
+-rw-r--r--   0        0        0      468 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_keyword_decorator_and_other_decorator/foo.py
+-rw-r--r--   0        0        0      162 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_keyword_with_conflicting_name.robot
+-rw-r--r--   0        0        0       62 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_line_number.robot
+-rw-r--r--   0        0        0      535 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_listener_calls_log_file/Listener.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_listener_calls_log_file/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_listener_calls_log_file/foo.robot
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_nested_keyword_that_fails/__init__.py
+-rw-r--r--   0        0        0       71 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_nested_keyword_that_fails/bar.robot
+-rw-r--r--   0        0        0      160 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_nested_keyword_that_fails/foo.py
+-rw-r--r--   0        0        0       40 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_no_tests_found_when_tests_exist.robot
+-rw-r--r--   0        0        0       32 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_one_test_fails.robot
+-rw-r--r--   0        0        0       36 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_one_test_passes.robot
+-rw-r--r--   0        0        0       32 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_one_test_skipped.robot
+-rw-r--r--   0        0        0       61 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_parameterized_tags/foo.robot
+-rw-r--r--   0        0        0       34 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_parameterized_tags/tox.ini
+-rw-r--r--   0        0        0       95 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_run_keyword_and_ignore_error.robot
+-rw-r--r--   0        0        0       38 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_run_two_files/a.robot
+-rw-r--r--   0        0        0       38 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_run_two_files/b.robot
+-rw-r--r--   0        0        0      115 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_setup_fails.robot
+-rw-r--r--   0        0        0      111 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_setup_passes.robot
+-rw-r--r--   0        0        0      107 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_setup_skipped.robot
+-rw-r--r--   0        0        0      163 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_setup_with_args.robot
+-rw-r--r--   0        0        0       96 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_tags.robot
+-rw-r--r--   0        0        0      100 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_tags_in_settings.robot
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_tags_with_kwargs/__init__.py
+-rw-r--r--   0        0        0      722 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_tags_with_kwargs/conftest.py
+-rw-r--r--   0        0        0       93 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_tags_with_kwargs/test_tags_with_kwargs.robot
+-rw-r--r--   0        0        0      119 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_teardown_fails.robot
+-rw-r--r--   0        0        0      115 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_teardown_passes.robot
+-rw-r--r--   0        0        0      111 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_teardown_skipped.robot
+-rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_traceback/__init__.py
+-rw-r--r--   0        0        0       72 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_traceback/test.robot
+-rw-r--r--   0        0        0       78 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_traceback/util.py
+-rw-r--r--   0        0        0       36 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_two_files_run_one_test/bar.robot
+-rw-r--r--   0        0        0       54 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_two_files_run_one_test/foo.robot
+-rw-r--r--   0        0        0       54 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_two_files_run_test_from_second_suite/asdf/foo.robot
+-rw-r--r--   0        0        0       36 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_two_files_run_test_from_second_suite/fdsa/bar.robot
+-rw-r--r--   0        0        0       55 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_two_tests_one_fail_one_pass.robot
+-rw-r--r--   0        0        0       57 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_warning_on_unknown_tag.robot
+-rw-r--r--   0        0        0     1035 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/test_common.py
+-rw-r--r--   0        0        0    34386 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/test_python.py
+-rw-r--r--   0        0        0    10909 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/test_robot.py
+-rw-r--r--   0        0        0     1286 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/test_robot_utils.py
+-rw-r--r--   0        0        0     1776 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/type_tests.py
+-rw-r--r--   0        0        0    18102 1970-01-01 00:00:00.000000 pytest_robotframework-4.2.0/PKG-INFO
```

### Comparing `pytest_robotframework-4.1.4/LICENSE` & `pytest_robotframework-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/README.md` & `pytest_robotframework-4.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,16 @@
 
 ## running tests in parallel
 
 running tests in parallel using [pytest-xdist](https://pytest-xdist.readthedocs.io/en/stable/) is supported. when running with xdist, pytest-robotframework will run separate instances of robot for each test, then merge the robot output files together automatically using rebot.
 
 # config
 
+pass `--capture=no` to make `logger.console` work properly. 
+
 since this is a pytest plugin, you should avoid using robot options that have pytest equivalents:
 
 | instead of...                           | use...                                | notes                                                                                                                                                   |
 | :-------------------------------------- | :------------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------ |
 | `robot --include tag_name`              | `pytest -m tag_name`                  |                                                                                                                                                         |
 | `robot --exclude tag_name`              | `pytest -m not tag_name`              |                                                                                                                                                         |
 | `robot --skip tag_name`                 | `pytest -m "not tag_name"`            |                                                                                                                                                         |
```

### Comparing `pytest_robotframework-4.1.4/pyproject.toml` & `pytest_robotframework-4.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytest_robotframework"
-version = "4.1.4"
+version = "4.2.0"
 description = "a pytest plugin that can run both python and robotframework tests while generating robot reports for them"
 authors = [
     { name = "DetachHead", email = "detachhead@users.noreply.github.com" },
 ]
 dependencies = [
     "pytest<9,>=7",
     "robotframework<8.0.0,>=6.1",
```

### Comparing `pytest_robotframework-4.1.4/pytest_robotframework/__init__.py` & `pytest_robotframework-4.2.0/pytest_robotframework/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/pytest_robotframework/_internal/cringe_globals.py` & `pytest_robotframework-4.2.0/pytest_robotframework/_internal/cringe_globals.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/pytest_robotframework/_internal/errors.py` & `pytest_robotframework-4.2.0/pytest_robotframework/_internal/errors.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/pytest_robotframework/_internal/pytest/plugin.py` & `pytest_robotframework-4.2.0/pytest_robotframework/_internal/pytest/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """the actual pytest plugin"""
 
 from __future__ import annotations
 
+import contextlib
+import os
 from ast import Assert, Call, Constant, Expr, If, Raise, copy_location, stmt
 from pathlib import Path
+from typing import IO
 
 import pytest
 from _pytest.assertion import rewrite
 from _pytest.assertion.rewrite import (
     AssertionRewriter,
     _get_assertion_exprs,  # pyright:ignore[reportPrivateUsage]
     traverse_node,
 )
 from _pytest.main import resolve_collection_argument
 from pytest import (
     Collector,
+    Config,
     StashKey,
     TempPathFactory,
     TestReport,
     hookimpl,
     version_tuple as pytest_version,
 )
 from robot.api import logger
@@ -77,14 +81,15 @@
     robot_6,
 )
 from pytest_robotframework._internal.utils import patch_method
 
 if TYPE_CHECKING:
     from types import TracebackType
 
+    from _pytest.terminal import TerminalReporter
     from pluggy import PluginManager
     from pytest import CallInfo, Item, Parser, Session
 
 
 _explanation_key = StashKey[str]()
 
 
@@ -310,14 +315,15 @@
     robot_options = {
         "report": None,
         "output": None,
         "log": None,
         "exitonerror": True,
         "prerunmodifier": [RobotSuiteCollector(session)],
         "listener": None,
+        "console": "none",
     }
     _run_robot(session, robot_options)
 
 
 def _robot_run_tests(session: Session, xdist_item: Item | None = None):
     """
     runs robot either on an individual item or on every item in the session.
@@ -432,61 +438,75 @@
             def option_names(settings: Mapping[str, tuple[str, object]]) -> list[str]:
                 return [value[0] for value in settings.values()]
 
             outputs = list(_xdist_temp_dir(session).glob(f"*/{_xdist_ourput_dir_name}/*.xml"))
             # if there were no outputs there were probably no tests run or some other error occured,
             # so silently skip this
             if outputs:
-                rebot = Rebot()
-                # if tests from different suites were run, the top level suite can have a different
-                # name. rebot will refuse to merge if the top level suite names don't match, so we
-                # need to set them all to the same name before merging them.
-                if len(outputs) > 1:
-                    merged_suite_name = cast(str, ExecutionResult(*outputs).suite.name)  # pyright:ignore[reportUnknownMemberType]
-                    for output in outputs:
-                        _ = cast(int, rebot.main([output], output=output, name=merged_suite_name))  # pyright:ignore[reportUnknownMemberType]
-                rebot_options = merge_robot_options(
-                    {
-                        # rebot doesn't recreate the output.xml unless you sepecify it
-                        # explicitly. we want to do this because our usage of rebot is an
-                        # implementation detail and we want the output to appear the same
-                        # regardless of whether the user is running with xdist
-                        "output": "output.xml"
-                    },
-                    {
-                        # filter out any robot args that aren't valid rebot args
-                        key: value
-                        for key, value in robot_args.items()
-                        if key
-                        in option_names(
-                            RebotSettings._extra_cli_opts  # pyright:ignore[reportPrivateUsage]
-                        )
-                        or key
-                        in option_names(
-                            _BaseSettings._cli_opts  # pyright:ignore[reportPrivateUsage,reportUnknownArgumentType,reportUnknownMemberType]
-                        )
-                    },
-                )
-
-                # we need to always set the loglevel to TRACE, despite whatever it was set to
-                # when running robot. otherwise if the loglevel was changed to DEBUG or TRACE
-                # programmatically inside a test, they would not appear in the merged output
-                log_level_value = robot_args["loglevel"]
-                default_log_level = (
-                    log_level_value.split(":")[1] if ":" in log_level_value else "INFO"
-                )
-                rebot_options["loglevel"] = f"TRACE:{default_log_level}"
 
-                _ = rebot.main(  # pyright:ignore[reportUnknownVariableType,reportUnknownMemberType]
-                    outputs,
-                    # merge is deliberately specified here instead of in the merged dict because it
-                    # should never be overwritten
-                    merge=True,
-                    **rebot_options,
-                )
+                def redirector(file: IO[str]) -> contextlib._RedirectStream[IO[str]]:  # pyright: ignore[reportPrivateUsage]
+                    # Here we create a jenkem huffer because you can't control rebots console output
+                    #  Rebot uses __stdout__, which doesn't have an implementation in contextlib
+                    result = contextlib._RedirectStream(file)  # pyright: ignore[reportPrivateUsage]
+                    result._stream = "__stdout__"  # pyright: ignore[reportAttributeAccessIssue]
+                    return result
+
+                with Path(os.devnull).open("w", encoding="UTF8") as devull, redirector(devull):
+                    rebot = Rebot()
+                    # if tests from different suites were run, the top level suite can have a
+                    # different name. rebot will refuse to merge if the top level suite names
+                    # don't match, so we need to set them all to the same name before merging them.
+                    if len(outputs) > 1:
+                        merged_suite_name = cast(str, ExecutionResult(*outputs).suite.name)  # pyright:ignore[reportUnknownMemberType]
+                        for output in outputs:
+                            _ = cast(
+                                int,
+                                rebot.main(  # pyright:ignore[reportUnknownMemberType]
+                                    [output], output=output, name=merged_suite_name, stdout=None
+                                ),
+                            )
+                    rebot_options = merge_robot_options(
+                        {
+                            # rebot doesn't recreate the output.xml unless you sepecify it
+                            # explicitly. we want to do this because our usage of rebot is an
+                            # implementation detail and we want the output to appear the same
+                            # regardless of whether the user is running with xdist
+                            "output": "output.xml"
+                        },
+                        {
+                            # filter out any robot args that aren't valid rebot args
+                            key: value
+                            for key, value in robot_args.items()
+                            if key
+                            in option_names(
+                                RebotSettings._extra_cli_opts  # pyright:ignore[reportPrivateUsage]
+                            )
+                            or key
+                            in option_names(
+                                _BaseSettings._cli_opts  # pyright:ignore[reportPrivateUsage,reportUnknownArgumentType,reportUnknownMemberType]
+                            )
+                        },
+                    )
+
+                    # we need to always set the loglevel to TRACE, despite whatever it was set to
+                    # when running robot. otherwise if the loglevel was changed to DEBUG or TRACE
+                    # programmatically inside a test, they would not appear in the merged output
+                    log_level_value = robot_args["loglevel"]
+                    default_log_level = (
+                        log_level_value.split(":")[1] if ":" in log_level_value else "INFO"
+                    )
+                    rebot_options["loglevel"] = f"TRACE:{default_log_level}"
+
+                    _ = rebot.main(  # pyright:ignore[reportUnknownVariableType,reportUnknownMemberType]
+                        outputs,
+                        # merge is deliberately specified here instead of in the merged dict because
+                        # it should never be overwritten
+                        merge=True,
+                        **rebot_options,
+                    )
             else:
                 # this means robot was never run in any of the workers because there was no items,
                 # so we run it here to generate an empty log file to be consistent with what would
                 # happen when running with no items without xdist
                 _robot_run_tests(session)
         yield
     finally:
@@ -626,12 +646,21 @@
 def pytest_runtest_protocol(item: Item):
     if is_xdist_worker(item.session):
         _robot_run_tests(item.session, xdist_item=item)
         return True
     return None
 
 
+@hookimpl(tryfirst=True)
+def pytest_terminal_summary(terminalreporter: TerminalReporter, config: Config):
+    log_file = config.rootpath / cast(str, config.option.robot_log)  # pyright: ignore[reportAny]
+    terminalreporter.line("")
+    terminalreporter.line("Robot Framework Output Files:", bold=True)
+    terminalreporter.line(f"Log:     {log_file}")
+    terminalreporter.line(f"Log URI: {log_file.as_uri()}")
+
+
 @patch_method(ErrorDetails)
 def _is_robot_traceback(  # pyright: ignore[reportUnusedFunction]
     _old_method: object, _self: ErrorDetails, tb: TracebackType
 ) -> bool | str | None:
     return is_robot_traceback(tb)
```

### Comparing `pytest_robotframework-4.1.4/pytest_robotframework/_internal/pytest/xdist_utils.py` & `pytest_robotframework-4.2.0/pytest_robotframework/_internal/pytest/xdist_utils.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/pytest_robotframework/_internal/robot/library.py` & `pytest_robotframework-4.2.0/pytest_robotframework/_internal/robot/library.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/pytest_robotframework/_internal/robot/listeners_and_suite_visitors.py` & `pytest_robotframework-4.2.0/pytest_robotframework/_internal/robot/listeners_and_suite_visitors.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/pytest_robotframework/_internal/robot/utils.py` & `pytest_robotframework-4.2.0/pytest_robotframework/_internal/robot/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     cast,
 )
 
 from basedtyping import T
 from pytest import Item, Session, StashKey
 from robot import model, running
 from robot.api.interfaces import ListenerV2, ListenerV3, Parser
-from robot.conf.settings import _BaseSettings  # pyright:ignore[reportPrivateUsage]
+from robot.conf.settings import RobotSettings, _BaseSettings  # pyright:ignore[reportPrivateUsage]
 from robot.running.context import _ExecutionContext  # pyright:ignore[reportPrivateUsage]
 from robot.version import VERSION
 from typing_extensions import override
 
 from pytest_robotframework._internal.utils import main_package_name
 
 if TYPE_CHECKING:
@@ -94,14 +94,16 @@
     listener: list[str | Listener]
     statusrc: bool
     skipteardownonexit: bool
     prerunmodifier: list[str | model.SuiteVisitor]
     prerebotmodifier: list[str | model.SuiteVisitor]
     randomize: Literal["ALL", "SUITES", "TESTS", "NONE"]
     console: Literal["verbose", "dotted", "quiet", "none"]
+    """the default in robot is `"verbose", however pytest-robotframework changes the default to
+    `"quiet"`, if you change this, then pytest and robot outputs will overlap."""
     dotted: bool
     quiet: bool
     consolewidth: int
     consolecolors: Literal["AUTO", "ON", "ANSI", "OFF"]
     consolemarkers: Literal["AUTO", "ON", "OFF"]
     pythonpath: list[str]
     # argumentfile is not supported because it's not in the _cli_opts dict for some reason
@@ -176,15 +178,17 @@
             return item
     # the robot test was found but got filtered out by pytest, or if
     # all_items_should_have_tests=False then it was in a different worker
     return None
 
 
 def full_test_name(test: ModelTestCase) -> str:
-    return test.name if robot_6 else test.full_name
+    # we cut out the top level suite name because it seems to change dynamically as more suites get
+    # collected, or something
+    return test.name if robot_6 else test.full_name.split(".", 1)[1]
 
 
 robot_errors_key = StashKey[List[str]]()
 
 
 def add_robot_error(item_or_session: Item | Session, message: str):
     if robot_errors_key not in item_or_session.stash:
@@ -237,14 +241,16 @@
 
 
 def cli_defaults(settings_class: Callable[[dict[str, object]], _BaseSettings]) -> RobotOptions:
     # need to reset outputdir because if anything from robot gets imported before pytest runs, then
     # the cwd gets updated, robot will still run with the outdated cwd.
     # we set it in this wacky way to make sure it never overrides user preferences
     _BaseSettings._cli_opts["OutputDir"] = ("outputdir", ".")  # pyright:ignore[reportUnknownMemberType,reportPrivateUsage]
+    # Need to set this so that there aren't two competing frameworks dumping into the console
+    RobotSettings._extra_cli_opts["ConsoleType"] = ("console", "quiet")  # pyright:ignore[reportUnknownMemberType,reportPrivateUsage,reportArgumentType]
     # https://github.com/DetachHead/basedpyright#note-about-casting-with-typeddicts
     return cast(  # pyright:ignore[reportInvalidCast]
         RobotOptions,
         dict(
             # instantiate the class because _BaseSettings.__init__ adds any additional opts
             # that the subclass may have defined (using _extra_cli_opts)
             settings_class(  # pyright:ignore[reportUnknownArgumentType,reportUnknownMemberType]
```

### Comparing `pytest_robotframework-4.1.4/pytest_robotframework/_internal/utils.py` & `pytest_robotframework-4.2.0/pytest_robotframework/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/pytest_robotframework/hooks.py` & `pytest_robotframework-4.2.0/pytest_robotframework/hooks.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/tests/conftest.py` & `pytest_robotframework-4.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/tests/fixtures/test_python/test_catch_errors_decorator/conftest.py` & `pytest_robotframework-4.2.0/tests/fixtures/test_python/test_catch_errors_decorator/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/conftest.py` & `pytest_robotframework-4.2.0/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/tests/fixtures/test_python/test_fixture_scope.py` & `pytest_robotframework-4.2.0/tests/fixtures/test_python/test_fixture_scope.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_doesnt_suppress.py` & `pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_doesnt_suppress.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_raises_in_body_and_exit.py` & `pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_raises_in_body_and_exit.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/tests/fixtures/test_python/test_listener_calls_log_file/Listener.py` & `pytest_robotframework-4.2.0/tests/fixtures/test_python/test_listener_calls_log_file/Listener.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/tests/fixtures/test_python/test_listener_not_run_during_collection/conftest.py` & `pytest_robotframework-4.2.0/tests/fixtures/test_python/test_listener_not_run_during_collection/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/conftest.py` & `pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_listener_calls_log_file/Listener.py` & `pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_listener_calls_log_file/Listener.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/tests/fixtures/test_robot/test_tags_with_kwargs/conftest.py` & `pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_tags_with_kwargs/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/tests/test_common.py` & `pytest_robotframework-4.2.0/tests/test_common.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,7 +19,12 @@
 
 # i don't care to maintain multiple versions of this type so only test against the latest version
 @mark.skipif(robot_6, reason="old robot version")
 def test_robot_options_type_is_up_to_date():
     assert {key for key in cli_defaults(RobotSettings) if key not in banned_options} == set(
         RobotOptions.__annotations__.keys()
     )
+
+
+def test_robot_file_and_python_file(pr: PytestRobotTester):
+    pr.run_and_assert_result("foo.robot", "test_bar.py", passed=2)
+    pr.assert_log_file_exists()
```

### Comparing `pytest_robotframework-4.1.4/tests/test_python.py` & `pytest_robotframework-4.2.0/tests/test_python.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from __future__ import annotations
 
+import re
+import sys
 from pathlib import Path
 from re import search
 from typing import TYPE_CHECKING, List, cast
 
+from _pytest.assertion.util import running_on_ci
 from pytest import ExitCode, MonkeyPatch
 
+from pytest_robotframework._internal.robot.utils import robot_6
 from tests.conftest import (
     PytestRobotTester,
     XmlElement,
     assert_robot_total_stats,
     output_xml,
     xpath,
 )
@@ -42,14 +46,19 @@
 
 
 def test_two_tests_two_files_one_fail_one_pass(pr: PytestRobotTester):
     pr.run_and_assert_result(passed=1, failed=1)
     pr.assert_log_file_exists()
 
 
+def test_run_two_files(pr: PytestRobotTester):
+    pr.run_and_assert_result("test_a.py", "test_b.py", passed=2)
+    pr.assert_log_file_exists()
+
+
 def test_two_tests_with_same_name_one_fail_one_pass(pr: PytestRobotTester):
     pr.run_and_assert_result(passed=1, failed=1)
     pr.assert_log_file_exists()
 
 
 def test_suites(pr: PytestRobotTester):
     pr.run_and_assert_result(passed=1)
@@ -880,7 +889,49 @@
     pr.run_and_assert_assert_pytest_result("--collect-only", exit_code=ExitCode.NO_TESTS_COLLECTED)
 
 
 def test_class_three_tests_one_fail(pr: PytestRobotTester):
     """this test is for an xdist issue. needs to have one more tests than there are workers"""
     pr.run_and_assert_result(passed=2, failed=1)
     pr.assert_log_file_exists()
+
+
+def test_console_summary(pr: PytestRobotTester):
+    result = pr.run_pytest(subprocess=True)
+    path = pr.pytester.path / "log.html"
+    assert re.search(
+        rf"""
+
+Robot Framework Output Files:
+Log:     {re.escape(str(path))}
+Log URI: {re.escape(path.as_uri())}
+""",
+        "\n".join(result.outlines),
+    )
+
+
+def test_console_output(pr: PytestRobotTester):
+    if pr.xdist:
+        result = pr.run_pytest("--capture=no")
+        assert "Output:" not in "\n".join(result.outlines)
+    else:
+        result = pr.run_pytest("--collect-only")
+        assert "0 tests, 0 passed, 0 failed" not in result.outlines
+        assert "Output:  None" not in result.outlines
+
+        result = pr.run_pytest("--capture=no", "--collect-only")
+        assert "0 tests, 0 passed, 0 failed" not in result.outlines
+        assert "Output:  None" not in result.outlines
+
+        result = pr.run_pytest("--capture=no")
+        if sys.platform == "win32" and running_on_ci():
+            # don't ask
+            assert "I'm console ?" in result.outlines
+        else:
+            assert "I'm console 🚽" in result.outlines
+        assert "[ WARN ] I'm warning" in result.errlines
+
+        result = pr.run_pytest("--quiet", "--capture=no", "--robot-console=verbose")
+        if robot_6:
+            assert f"Output:  {pr.pytester.path / 'output.xml'}" in result.outlines
+        else:
+            assert "Output:  output.xml" in result.outlines
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytest_robotframework-4.1.4/tests/test_robot.py` & `pytest_robotframework-4.2.0/tests/test_robot.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,19 @@
     xml = output_xml()
     assert xml.xpath("./suite//test[@name='Baz']/status[@status='PASS']")
     assert xml.xpath("./suite//test[@name='Baz']/kw/status[@status='PASS']")
     assert not xml.xpath("./suite//test[@name='Foo']")
     assert not xml.xpath("./suite//test[@name='Bar']")
 
 
+def test_run_two_files(pr: PytestRobotTester):
+    pr.run_and_assert_result("a.robot", "b.robot", passed=2)
+    pr.assert_log_file_exists()
+
+
 def test_tags(pr: PytestRobotTester):
     pr.run_and_assert_result("-m", "m1", passed=1)
     pr.assert_log_file_exists()
     xml = output_xml()
     assert xml.xpath(".//test[@name='Foo']/tag[.='m1']")
     assert not xml.xpath(".//test[@name='Bar']")
 
@@ -288,7 +293,16 @@
     # keyword is over we want to make sure it's not printed multiple times
     assert xpath(xml, "//msg[@level='FAIL']")
 
 
 def test_fails_when_import_error_and_exit_on_error(pr: PytestRobotTester):
     pr.run_and_assert_assert_pytest_result("--robot-exitonerror", exit_code=ExitCode.INTERNAL_ERROR)
     assert_robot_total_stats(failed=1)
+
+
+def test_traceback(pr: PytestRobotTester):
+    result = pr.run_pytest("--tb=short")
+    assert """
+util.py:5: in thing
+    raise Exception("asdf")
+E   Exception: asdf
+""" in "\n".join(result.outlines)
```

### Comparing `pytest_robotframework-4.1.4/tests/test_robot_utils.py` & `pytest_robotframework-4.2.0/tests/test_robot_utils.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/tests/type_tests.py` & `pytest_robotframework-4.2.0/tests/type_tests.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.4/PKG-INFO` & `pytest_robotframework-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_robotframework
-Version: 4.1.4
+Version: 4.2.0
 Summary: a pytest plugin that can run both python and robotframework tests while generating robot reports for them
 Author-Email: DetachHead <detachhead@users.noreply.github.com>
 License: MIT
 Project-URL: Repository, https://github.com/detachhead/pytest-robotframework
 Requires-Python: <4.0,>=3.8
 Requires-Dist: pytest<9,>=7
 Requires-Dist: robotframework<8.0.0,>=6.1
@@ -164,14 +164,16 @@
 
 ## running tests in parallel
 
 running tests in parallel using [pytest-xdist](https://pytest-xdist.readthedocs.io/en/stable/) is supported. when running with xdist, pytest-robotframework will run separate instances of robot for each test, then merge the robot output files together automatically using rebot.
 
 # config
 
+pass `--capture=no` to make `logger.console` work properly. 
+
 since this is a pytest plugin, you should avoid using robot options that have pytest equivalents:
 
 | instead of...                           | use...                                | notes                                                                                                                                                   |
 | :-------------------------------------- | :------------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------ |
 | `robot --include tag_name`              | `pytest -m tag_name`                  |                                                                                                                                                         |
 | `robot --exclude tag_name`              | `pytest -m not tag_name`              |                                                                                                                                                         |
 | `robot --skip tag_name`                 | `pytest -m "not tag_name"`            |                                                                                                                                                         |
```

