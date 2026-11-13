# 验收结果

passed

MIR：通过，但有 4 项缺 MIR

全部必需检查已通过，主 body BB 全覆盖。公开报告省略本机命令与日志路径。

```json
{
  "status": "passed",
  "passed": true,
  "clean_pass": false,
  "mir_status": "通过，但有 4 项缺 MIR",
  "missing_mir_count": 4,
  "counts": {
    "action_count": 27,
    "bb_covered": 658,
    "bb_total": 658,
    "execution_node_count": 56,
    "goal_count": 8,
    "message_count": 76,
    "phase_count": 4
  },
  "browser_checked": true,
  "checks_not_run": [],
  "checks": {
    "batch": {
      "passed": true
    },
    "batch-reference": {
      "passed": true
    },
    "browser": {
      "passed": true
    },
    "contract": {
      "passed": true
    },
    "duplicates": {
      "passed": true
    },
    "hard-rules": {
      "passed": true
    },
    "independent-source": {
      "passed": true
    },
    "principles": {
      "passed": true
    },
    "regressions": {
      "passed": true
    }
  },
  "source_commit": "c248f6d48b97eb4a2aa56147a0b11b7d763278b9",
  "registered_deviation_count": 0,
  "missing_mir": [
    {
      "callee": "<dyn tools::registry::CoreToolRuntime as tools::registry::CoreToolRuntime>::matches_kind",
      "category": "declaration",
      "def_path_hash": "0324eb8659b5ab567f347cbdcc2b778a",
      "reason": "dynamic dispatch has no concrete body",
      "source_line": "core/src/tools/registry.rs:585"
    },
    {
      "callee": "std::option::Option::<state::turn::ActiveTurn>::as_mut",
      "category": "declaration",
      "def_path_hash": "0403f53630f0138e2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:545"
    },
    {
      "callee": "std::option::Option::<tools::control_tool_analytics::ControlToolCallGuard<'_>>::as_mut",
      "category": "declaration",
      "def_path_hash": "0403f53630f0138e2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:702"
    },
    {
      "callee": "std::boxed::Box::<tools::registry::PostToolUseFeedbackOutput>::new",
      "category": "declaration",
      "def_path_hash": "0ea4ff1e37caac6e0881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:765"
    },
    {
      "callee": "std::option::Option::<std::string::String>::as_deref",
      "category": "declaration",
      "def_path_hash": "1835c87e5e8cca882bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:538"
    },
    {
      "callee": "std::option::Option::<std::sync::Arc<tools::context::ToolCallState>>::as_deref",
      "category": "declaration",
      "def_path_hash": "1835c87e5e8cca882bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:622"
    },
    {
      "callee": "std::option::Option::<std::sync::Arc<tools::context::ToolCallState>>::as_deref",
      "category": "declaration",
      "def_path_hash": "1835c87e5e8cca882bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:642"
    },
    {
      "callee": "std::option::Option::<std::sync::Arc<tools::context::ToolCallState>>::as_deref",
      "category": "declaration",
      "def_path_hash": "1835c87e5e8cca882bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:689"
    },
    {
      "callee": "std::option::Option::<std::sync::Arc<tools::context::ToolCallState>>::as_deref",
      "category": "declaration",
      "def_path_hash": "1835c87e5e8cca882bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:750"
    },
    {
      "callee": "core::slice::<impl [codex_protocol::parse_command::ParsedCommand]>::iter",
      "category": "declaration",
      "def_path_hash": "1c7fe2d1b3afe1292bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:666"
    },
    {
      "callee": "<&str as std::cmp::PartialEq>::eq",
      "category": "declaration",
      "def_path_hash": "20f42b1508b59b242bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:673"
    },
    {
      "callee": "<str as std::cmp::PartialEq>::eq",
      "category": "declaration",
      "def_path_hash": "20f42b1508b59b242bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:579"
    },
    {
      "callee": "<impl Display as std::string::ToString>::to_string",
      "category": "declaration",
      "def_path_hash": "227cbef13c3894950881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "rollout-trace/src/tool_dispatch.rs:188"
    },
    {
      "callee": "<str as std::string::ToString>::to_string",
      "category": "declaration",
      "def_path_hash": "227cbef13c3894950881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:724"
    },
    {
      "callee": "<dyn tools::registry::CoreToolRuntime as tools::registry::CoreToolRuntime>::telemetry_tags",
      "category": "declaration",
      "def_path_hash": "2fb71021381af76e7f347cbdcc2b778a",
      "reason": "dynamic dispatch has no concrete body",
      "source_line": "core/src/tools/registry.rs:574"
    },
    {
      "callee": "<tokio::sync::MutexGuard<'_, state::turn::TurnState> as std::ops::DerefMut>::deref_mut",
      "category": "declaration",
      "def_path_hash": "373c81559cdd983c2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:547"
    },
    {
      "callee": "<tokio::sync::MutexGuard<'_, std::option::Option<state::turn::ActiveTurn>> as std::ops::DerefMut>::deref_mut",
      "category": "declaration",
      "def_path_hash": "373c81559cdd983c2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:545"
    },
    {
      "callee": "<std::borrow::Cow<'_, str> as std::convert::AsRef<str>>::as_ref",
      "category": "declaration",
      "def_path_hash": "39d972858970f2b32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:562"
    },
    {
      "callee": "<std::borrow::Cow<'_, str> as std::convert::AsRef<str>>::as_ref",
      "category": "declaration",
      "def_path_hash": "39d972858970f2b32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:591"
    },
    {
      "callee": "<std::borrow::Cow<'_, str> as std::convert::AsRef<str>>::as_ref",
      "category": "declaration",
      "def_path_hash": "39d972858970f2b32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:686"
    },
    {
      "callee": "<std::boxed::Box<dyn codex_tools::ToolOutput> as std::convert::AsRef<dyn codex_tools::ToolOutput>>::as_ref",
      "category": "declaration",
      "def_path_hash": "39d972858970f2b32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:774"
    },
    {
      "callee": "<std::boxed::Box<dyn codex_tools::ToolOutput> as std::convert::AsRef<dyn codex_tools::ToolOutput>>::as_ref",
      "category": "declaration",
      "def_path_hash": "39d972858970f2b32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:779"
    },
    {
      "callee": "<std::sync::Arc<dyn tools::registry::CoreToolRuntime> as std::convert::AsRef<dyn tools::registry::CoreToolRuntime>>::as_ref",
      "category": "declaration",
      "def_path_hash": "39d972858970f2b32bac9d628bdc1eb8",
      "reason": "dynamic dispatch has no concrete body",
      "source_line": "core/src/tools/registry.rs:689"
    },
    {
      "callee": "<std::sync::Arc<session::step_context::StepContext> as std::convert::AsRef<session::step_context::StepContext>>::as_ref",
      "category": "declaration",
      "def_path_hash": "39d972858970f2b32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:606"
    },
    {
      "callee": "<std::sync::Arc<session::step_context::StepContext> as std::convert::AsRef<session::step_context::StepContext>>::as_ref",
      "category": "declaration",
      "def_path_hash": "39d972858970f2b32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:722"
    },
    {
      "callee": "core::num::<impl u64>::saturating_add",
      "category": "declaration",
      "def_path_hash": "3d991b8e52dc11bf2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:547"
    },
    {
      "callee": "std::result::Result::<tools::registry::AnyToolResult, codex_tools::FunctionCallError>::as_ref",
      "category": "declaration",
      "def_path_hash": "4508164c71afc03d2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:711"
    },
    {
      "callee": "memory_usage::shell_script_for_invocation",
      "category": "out-of-scope",
      "def_path_hash": "47d0b0a078c3bb3d7f347cbdcc2b778a",
      "reason": "definition exists but extraction container has no body (body_available=True)",
      "rerun_command": "python3 \"$MIRLOADER_ROOT/mirloader.py\" --definitions '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/posts/codex-context/v3/v3-1-2-claude/03outputs/definitions/definitions.json' --scope \"$MIR_SCOPE_WITH_MISSING_DEFINITIONS\" --workspace '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/codex/codex-rs' --output-dir \"$MIR_REEXTRACT_OUTPUT\" --result-file \"$MIR_REEXTRACT_OUTPUT/mir-bodies.json\" --offline --jobs 8",
      "scope_requirement": "Generate a scope-definitions JSON including memory_usage::shell_script_for_invocation (47d0b0a078c3bb3d7f347cbdcc2b778a); --scope accepts a scope file, not a callee name.",
      "source_line": "core/src/tools/registry.rs:664",
      "tool_reference": "$HOME/ai/codex拆解/v3/v3-1-2-claude/02scrpits/03-mir-extraction/mirloader/README.md"
    },
    {
      "callee": "core::bool::<impl bool>::then::<tools::control_tool_analytics::ControlToolCallGuard<'_>, {closure@core/src/tools/registry.rs:662:19: 662:21}>",
      "category": "declaration",
      "def_path_hash": "48691b4527624f622bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:660"
    },
    {
      "callee": "<std::boxed::Box<dyn codex_tools::ToolOutput> as codex_tools::ToolOutput>::success_for_logging",
      "category": "declaration",
      "def_path_hash": "55fd7e5e4abe6e3cb95c18fb6b5909c0",
      "reason": "dynamic dispatch has no concrete body",
      "source_line": "core/src/tools/registry.rs:693"
    },
    {
      "callee": "<std::boxed::Box<dyn codex_tools::ToolOutput> as codex_tools::ToolOutput>::success_for_logging",
      "category": "declaration",
      "def_path_hash": "55fd7e5e4abe6e3cb95c18fb6b5909c0",
      "reason": "dynamic dispatch has no concrete body",
      "source_line": "core/src/tools/registry.rs:699"
    },
    {
      "callee": "<std::iter::Map<std::slice::Iter<'_, codex_protocol::parse_command::ParsedCommand>, {closure@core/src/tools/registry.rs:666:52: 666:61}> as std::iter::Iterator>::all::<{closure@core/src/tools/registry.rs:673:47: 673:57}>",
      "category": "declaration",
      "def_path_hash": "579cd549bce9cc472bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:673"
    },
    {
      "callee": "std::pin::Pin::<&mut {async fn body of codex_otel::SessionTelemetry::log_tool_result_with_tags<tools::registry::AnyToolResult, {closure@core/src/tools/registry.rs:689:17: 689:19}, {async fn body of tools::registry::handle_any_tool()}, codex_tools::FunctionCallError, {closure@core/src/tools/registry.rs:690:17: 690:25}>()}>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:697 (macro)"
    },
    {
      "callee": "std::pin::Pin::<&mut {async fn body of hook_runtime::record_additional_contexts()}>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:740 (macro)"
    },
    {
      "callee": "std::pin::Pin::<&mut {async fn body of hook_runtime::run_post_tool_use_hooks()}>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:729 (macro)"
    },
    {
      "callee": "std::pin::Pin::<&mut {async fn body of hook_runtime::run_pre_tool_use_hooks()}>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:611 (macro)"
    },
    {
      "callee": "std::pin::Pin::<&mut {async fn body of tokio::sync::Mutex<state::turn::TurnState>::lock()}>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:546 (macro)"
    },
    {
      "callee": "std::pin::Pin::<&mut {async fn body of tokio::sync::Mutex<std::option::Option<state::turn::ActiveTurn>>::lock()}>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:544 (macro)"
    },
    {
      "callee": "std::pin::Pin::<&mut {async fn body of tools::lifecycle::notify_tool_start()}>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:658 (macro)"
    },
    {
      "callee": "std::pin::Pin::<&mut {async fn body of tools::registry::notify_tool_finish_if_unclaimed()}>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:625 (macro)"
    },
    {
      "callee": "std::pin::Pin::<&mut {async fn body of tools::registry::notify_tool_finish_if_unclaimed()}>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:647 (macro)"
    },
    {
      "callee": "std::pin::Pin::<&mut {async fn body of tools::registry::notify_tool_finish_if_unclaimed()}>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:751 (macro)"
    },
    {
      "callee": "codex_shell_command::parse_command::parse_shell_script",
      "category": "out-of-scope",
      "def_path_hash": "58a922a377bbcbbe1d8cb53fec2e5dae",
      "reason": "definition exists but extraction container has no body (body_available=True)",
      "rerun_command": "python3 \"$MIRLOADER_ROOT/mirloader.py\" --definitions '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/posts/codex-context/v3/v3-1-2-claude/03outputs/definitions/definitions.json' --scope \"$MIR_SCOPE_WITH_MISSING_DEFINITIONS\" --workspace '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/codex/codex-rs' --output-dir \"$MIR_REEXTRACT_OUTPUT\" --result-file \"$MIR_REEXTRACT_OUTPUT/mir-bodies.json\" --offline --jobs 8",
      "scope_requirement": "Generate a scope-definitions JSON including codex_shell_command::parse_command::parse_shell_script (58a922a377bbcbbe1d8cb53fec2e5dae); --scope accepts a scope file, not a callee name.",
      "source_line": "core/src/tools/registry.rs:665",
      "tool_reference": "$HOME/ai/codex拆解/v3/v3-1-2-claude/02scrpits/03-mir-extraction/mirloader/README.md"
    },
    {
      "callee": "<{async fn body of codex_otel::SessionTelemetry::log_tool_result_with_tags<tools::registry::AnyToolResult, {closure@core/src/tools/registry.rs:689:17: 689:19}, {async fn body of tools::registry::handle_any_tool()}, codex_tools::FunctionCallError, {closure@core/src/tools/registry.rs:690:17: 690:25}>()} as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:697 (macro)"
    },
    {
      "callee": "<{async fn body of hook_runtime::record_additional_contexts()} as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:740 (macro)"
    },
    {
      "callee": "<{async fn body of hook_runtime::run_post_tool_use_hooks()} as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:729 (macro)"
    },
    {
      "callee": "<{async fn body of hook_runtime::run_pre_tool_use_hooks()} as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:611 (macro)"
    },
    {
      "callee": "<{async fn body of tokio::sync::Mutex<state::turn::TurnState>::lock()} as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:546 (macro)"
    },
    {
      "callee": "<{async fn body of tokio::sync::Mutex<std::option::Option<state::turn::ActiveTurn>>::lock()} as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:544 (macro)"
    },
    {
      "callee": "<{async fn body of tools::lifecycle::notify_tool_start()} as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:658 (macro)"
    },
    {
      "callee": "<{async fn body of tools::registry::notify_tool_finish_if_unclaimed()} as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:625 (macro)"
    },
    {
      "callee": "<{async fn body of tools::registry::notify_tool_finish_if_unclaimed()} as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:647 (macro)"
    },
    {
      "callee": "<{async fn body of tools::registry::notify_tool_finish_if_unclaimed()} as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:751 (macro)"
    },
    {
      "callee": "std::option::Option::<&str>::is_none",
      "category": "declaration",
      "def_path_hash": "5d286d68af91d5e62bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:657"
    },
    {
      "callee": "<dyn tools::registry::CoreToolRuntime as tools::registry::CoreToolRuntime>::is_builtin_control_tool",
      "category": "declaration",
      "def_path_hash": "5f8eb5cd60dafbb97f347cbdcc2b778a",
      "reason": "dynamic dispatch has no concrete body",
      "source_line": "core/src/tools/registry.rs:614"
    },
    {
      "callee": "<dyn tools::registry::CoreToolRuntime as tools::registry::CoreToolRuntime>::is_builtin_control_tool",
      "category": "declaration",
      "def_path_hash": "5f8eb5cd60dafbb97f347cbdcc2b778a",
      "reason": "dynamic dispatch has no concrete body",
      "source_line": "core/src/tools/registry.rs:635"
    },
    {
      "callee": "<dyn tools::registry::CoreToolRuntime as tools::registry::CoreToolRuntime>::is_builtin_control_tool",
      "category": "declaration",
      "def_path_hash": "5f8eb5cd60dafbb97f347cbdcc2b778a",
      "reason": "dynamic dispatch has no concrete body",
      "source_line": "core/src/tools/registry.rs:660"
    },
    {
      "callee": "<dyn agent::api::AgentControl as agent::api::AgentControl>::identity",
      "category": "declaration",
      "def_path_hash": "60be2f337b0349f47f347cbdcc2b778a",
      "reason": "dynamic dispatch has no concrete body",
      "source_line": "core/src/session/session.rs:652"
    },
    {
      "callee": "std::fmt::Arguments::<'_>::new::<33, 1>",
      "category": "declaration",
      "def_path_hash": "6488302cb95ba4ee2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.rustup/toolchains/nightly-2026-03-01-aarch64-apple-darwin/lib/rustlib/src/rust/library/alloc/src/macros.rs:114"
    },
    {
      "callee": "std::fmt::Arguments::<'_>::new::<43, 1>",
      "category": "declaration",
      "def_path_hash": "6488302cb95ba4ee2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.rustup/toolchains/nightly-2026-03-01-aarch64-apple-darwin/lib/rustlib/src/rust/library/alloc/src/macros.rs:114 (macro)"
    },
    {
      "callee": "std::vec::Vec::<(&str, &str)>::with_capacity",
      "category": "declaration",
      "def_path_hash": "64ecb54f109897220881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:557"
    },
    {
      "callee": "std::vec::Vec::<(&str, &str)>::with_capacity",
      "category": "declaration",
      "def_path_hash": "64ecb54f109897220881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:575"
    },
    {
      "callee": "std::vec::Vec::<(&str, std::string::String)>::len",
      "category": "declaration",
      "def_path_hash": "66f475d433f123df0881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:575"
    },
    {
      "callee": "696fc50b7861b146714909b4a5023950",
      "category": "declaration",
      "def_path_hash": "696fc50b7861b146714909b4a5023950",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "?:None"
    },
    {
      "callee": "<&std::vec::Vec<(&str, std::string::String)> as std::iter::IntoIterator>::into_iter",
      "category": "declaration",
      "def_path_hash": "6b7aff59471188cd2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:578 (macro)"
    },
    {
      "callee": "std::vec::Vec::<(&str, &str)>::new",
      "category": "declaration",
      "def_path_hash": "70abb47554dd12f50881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:576"
    },
    {
      "callee": "<dyn tools::registry::CoreToolRuntime as tools::registry::CoreToolRuntime>::on_tool_result_accepted",
      "category": "declaration",
      "def_path_hash": "713618cb07b2fc927f347cbdcc2b778a",
      "reason": "dynamic dispatch has no concrete body",
      "source_line": "core/src/tools/registry.rs:774"
    },
    {
      "callee": "std::hint::must_use::<std::string::String>",
      "category": "declaration",
      "def_path_hash": "7502e9a8aa1e55562bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.rustup/toolchains/nightly-2026-03-01-aarch64-apple-darwin/lib/rustlib/src/rust/library/alloc/src/macros.rs:113"
    },
    {
      "callee": "std::hint::must_use::<std::string::String>",
      "category": "declaration",
      "def_path_hash": "7502e9a8aa1e55562bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.rustup/toolchains/nightly-2026-03-01-aarch64-apple-darwin/lib/rustlib/src/rust/library/alloc/src/macros.rs:113 (macro)"
    },
    {
      "callee": "std::option::Option::<std::string::String>::unwrap_or_else::<{closure@core/src/tools/registry.rs:757:79: 757:81}>",
      "category": "declaration",
      "def_path_hash": "7c70afa9f20534cc2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:757"
    },
    {
      "callee": "std::vec::Vec::<(&str, &str)>::push",
      "category": "declaration",
      "def_path_hash": "843c6065c71ce6170881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:580"
    },
    {
      "callee": "std::vec::Vec::<(&str, &str)>::push",
      "category": "declaration",
      "def_path_hash": "843c6065c71ce6170881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:582"
    },
    {
      "callee": "std::vec::Vec::<(&str, &str)>::push",
      "category": "declaration",
      "def_path_hash": "843c6065c71ce6170881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:677"
    },
    {
      "callee": "<std::iter::Map<std::slice::Iter<'_, codex_protocol::parse_command::ParsedCommand>, {closure@core/src/tools/registry.rs:666:52: 666:61}> as std::iter::Iterator>::next",
      "category": "declaration",
      "def_path_hash": "8bad2e8350701bdb2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:672"
    },
    {
      "callee": "<std::slice::Iter<'_, (&str, std::string::String)> as std::iter::Iterator>::next",
      "category": "declaration",
      "def_path_hash": "8bad2e8350701bdb2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:578 (macro)"
    },
    {
      "callee": "std::boxed::Box::<[codex_protocol::models::FunctionCallOutputContentItem; 1]>::new_uninit",
      "category": "declaration",
      "def_path_hash": "9073be98bf3d8cd10881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.rustup/toolchains/nightly-2026-03-01-aarch64-apple-darwin/lib/rustlib/src/rust/library/alloc/src/macros.rs:59"
    },
    {
      "callee": "std::slice::<impl [std::string::String]>::to_vec",
      "category": "declaration",
      "def_path_hash": "a10c8d820290eeca0881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:725"
    },
    {
      "callee": "<codex_protocol::SessionId as std::convert::Into<codex_protocol::ThreadId>>::into",
      "category": "declaration",
      "def_path_hash": "ab1a02cbfe5179c42bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/hook_runtime.rs:308"
    },
    {
      "callee": "std::fmt::format",
      "category": "declaration",
      "def_path_hash": "b4651e06de7cdf100881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.rustup/toolchains/nightly-2026-03-01-aarch64-apple-darwin/lib/rustlib/src/rust/library/alloc/src/macros.rs:114"
    },
    {
      "callee": "std::fmt::format",
      "category": "declaration",
      "def_path_hash": "b4651e06de7cdf100881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.rustup/toolchains/nightly-2026-03-01-aarch64-apple-darwin/lib/rustlib/src/rust/library/alloc/src/macros.rs:114 (macro)"
    },
    {
      "callee": "<dyn tools::registry::CoreToolRuntime as tools::registry::CoreToolRuntime>::with_updated_hook_input",
      "category": "declaration",
      "def_path_hash": "b823532a3be02e747f347cbdcc2b778a",
      "reason": "dynamic dispatch has no concrete body",
      "source_line": "core/src/tools/registry.rs:630"
    },
    {
      "callee": "<dyn tools::registry::CoreToolRuntime as tools::registry::CoreToolRuntime>::pre_tool_use_payload",
      "category": "declaration",
      "def_path_hash": "b98386d6fb5a15d87f347cbdcc2b778a",
      "reason": "dynamic dispatch has no concrete body",
      "source_line": "core/src/tools/registry.rs:603"
    },
    {
      "callee": "std::string::String::as_str",
      "category": "declaration",
      "def_path_hash": "c5047a448ff30a9f0881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:580"
    },
    {
      "callee": "std::string::String::as_str",
      "category": "declaration",
      "def_path_hash": "c5047a448ff30a9f0881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:582"
    },
    {
      "callee": "memory_usage::emit_metric_for_tool_read",
      "category": "out-of-scope",
      "def_path_hash": "cfc20e4f0a2492b17f347cbdcc2b778a",
      "reason": "definition exists but extraction container has no body (body_available=True)",
      "rerun_command": "python3 \"$MIRLOADER_ROOT/mirloader.py\" --definitions '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/posts/codex-context/v3/v3-1-2-claude/03outputs/definitions/definitions.json' --scope \"$MIR_SCOPE_WITH_MISSING_DEFINITIONS\" --workspace '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/codex/codex-rs' --output-dir \"$MIR_REEXTRACT_OUTPUT\" --result-file \"$MIR_REEXTRACT_OUTPUT/mir-bodies.json\" --offline --jobs 8",
      "scope_requirement": "Generate a scope-definitions JSON including memory_usage::emit_metric_for_tool_read (cfc20e4f0a2492b17f347cbdcc2b778a); --scope accepts a scope file, not a callee name.",
      "source_line": "core/src/tools/registry.rs:709",
      "tool_reference": "$HOME/ai/codex拆解/v3/v3-1-2-claude/02scrpits/03-mir-extraction/mirloader/README.md"
    },
    {
      "callee": "std::result::Result::<&tools::registry::AnyToolResult, &codex_tools::FunctionCallError>::ok",
      "category": "declaration",
      "def_path_hash": "d11f5e8c30506b3b2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:711"
    },
    {
      "callee": "<{async fn body of codex_otel::SessionTelemetry::log_tool_result_with_tags<tools::registry::AnyToolResult, {closure@core/src/tools/registry.rs:689:17: 689:19}, {async fn body of tools::registry::handle_any_tool()}, codex_tools::FunctionCallError, {closure@core/src/tools/registry.rs:690:17: 690:25}>()} as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:697 (macro)"
    },
    {
      "callee": "<{async fn body of hook_runtime::record_additional_contexts()} as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:740 (macro)"
    },
    {
      "callee": "<{async fn body of hook_runtime::run_post_tool_use_hooks()} as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:729 (macro)"
    },
    {
      "callee": "<{async fn body of hook_runtime::run_pre_tool_use_hooks()} as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:611 (macro)"
    },
    {
      "callee": "<{async fn body of tokio::sync::Mutex<state::turn::TurnState>::lock()} as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:546 (macro)"
    },
    {
      "callee": "<{async fn body of tokio::sync::Mutex<std::option::Option<state::turn::ActiveTurn>>::lock()} as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:544 (macro)"
    },
    {
      "callee": "<{async fn body of tools::lifecycle::notify_tool_start()} as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:658 (macro)"
    },
    {
      "callee": "<{async fn body of tools::registry::notify_tool_finish_if_unclaimed()} as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:625 (macro)"
    },
    {
      "callee": "<{async fn body of tools::registry::notify_tool_finish_if_unclaimed()} as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:647 (macro)"
    },
    {
      "callee": "<{async fn body of tools::registry::notify_tool_finish_if_unclaimed()} as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:751 (macro)"
    },
    {
      "callee": "std::boxed::box_assume_init_into_vec_unsafe::<codex_protocol::models::FunctionCallOutputContentItem, 1>",
      "category": "declaration",
      "def_path_hash": "dd172506adb50c350881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.rustup/toolchains/nightly-2026-03-01-aarch64-apple-darwin/lib/rustlib/src/rust/library/alloc/src/macros.rs:58"
    },
    {
      "callee": "<std::boxed::Box<dyn codex_tools::ToolOutput> as codex_tools::ToolOutput>::log_output",
      "category": "declaration",
      "def_path_hash": "e015398f0b49f57cb95c18fb6b5909c0",
      "reason": "dynamic dispatch has no concrete body",
      "source_line": "core/src/tools/registry.rs:692"
    },
    {
      "callee": "<codex_protocol::ToolName as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:532"
    },
    {
      "callee": "<std::string::String as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:533"
    },
    {
      "callee": "<std::string::String as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:607"
    },
    {
      "callee": "<std::vec::Vec<std::string::String> as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:738"
    },
    {
      "callee": "<tools::context::ToolInvocation as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:630"
    },
    {
      "callee": "<std::slice::Iter<'_, codex_protocol::parse_command::ParsedCommand> as std::iter::Iterator>::map::<&str, {closure@core/src/tools/registry.rs:666:52: 666:61}>",
      "category": "declaration",
      "def_path_hash": "e8ee9691c44e2ad32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:666"
    },
    {
      "callee": "<dyn tools::registry::CoreToolRuntime as tools::registry::CoreToolRuntime>::mcp_server_name",
      "category": "declaration",
      "def_path_hash": "e97d4516e6df1b7a7f347cbdcc2b778a",
      "reason": "dynamic dispatch has no concrete body",
      "source_line": "core/src/tools/registry.rs:657"
    },
    {
      "callee": "std::option::Option::<&tools::registry::AnyToolResult>::and_then::<tools::registry::PostToolUsePayload, {closure@core/src/tools/registry.rs:714:27: 714:35}>",
      "category": "declaration",
      "def_path_hash": "eb7d8a851e1450322bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:711"
    },
    {
      "callee": "sandbox_tags::SandboxTags::append_metric_tags",
      "category": "out-of-scope",
      "def_path_hash": "ed6dff1046ec9d6f7f347cbdcc2b778a",
      "reason": "definition exists but extraction container has no body (body_available=True)",
      "rerun_command": "python3 \"$MIRLOADER_ROOT/mirloader.py\" --definitions '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/posts/codex-context/v3/v3-1-2-claude/03outputs/definitions/definitions.json' --scope \"$MIR_SCOPE_WITH_MISSING_DEFINITIONS\" --workspace '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/codex/codex-rs' --output-dir \"$MIR_REEXTRACT_OUTPUT\" --result-file \"$MIR_REEXTRACT_OUTPUT/mir-bodies.json\" --offline --jobs 8",
      "scope_requirement": "Generate a scope-definitions JSON including sandbox_tags::SandboxTags::append_metric_tags (ed6dff1046ec9d6f7f347cbdcc2b778a); --scope accepts a scope file, not a callee name.",
      "source_line": "core/src/tools/registry.rs:558",
      "tool_reference": "$HOME/ai/codex拆解/v3/v3-1-2-claude/02scrpits/03-mir-extraction/mirloader/README.md"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:561"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:565"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:590"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:594"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:665"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:685"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:777"
    },
    {
      "callee": "<std::sync::Arc<config::Config> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:538"
    },
    {
      "callee": "<std::sync::Arc<dyn agent::api::AgentControl> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "dynamic dispatch has no concrete body",
      "source_line": "core/src/session/session.rs:652"
    },
    {
      "callee": "<std::sync::Arc<dyn tools::registry::CoreToolRuntime> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:574"
    },
    {
      "callee": "<std::sync::Arc<dyn tools::registry::CoreToolRuntime> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:585"
    },
    {
      "callee": "<std::sync::Arc<dyn tools::registry::CoreToolRuntime> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:603"
    },
    {
      "callee": "<std::sync::Arc<dyn tools::registry::CoreToolRuntime> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:614"
    },
    {
      "callee": "<std::sync::Arc<dyn tools::registry::CoreToolRuntime> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:630"
    },
    {
      "callee": "<std::sync::Arc<dyn tools::registry::CoreToolRuntime> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:635"
    },
    {
      "callee": "<std::sync::Arc<dyn tools::registry::CoreToolRuntime> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:657"
    },
    {
      "callee": "<std::sync::Arc<dyn tools::registry::CoreToolRuntime> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:660"
    },
    {
      "callee": "<std::sync::Arc<dyn tools::registry::CoreToolRuntime> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:774"
    },
    {
      "callee": "<std::sync::Arc<session::session::Session> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:544"
    },
    {
      "callee": "<std::sync::Arc<session::session::Session> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/tool_dispatch_trace.rs:26"
    },
    {
      "callee": "<std::sync::Arc<session::step_context::StepContext> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:534"
    },
    {
      "callee": "<std::sync::Arc<session::turn_context::TurnContext> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:538"
    },
    {
      "callee": "<std::sync::Arc<session::turn_context::TurnContext> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:541"
    },
    {
      "callee": "<std::sync::Arc<tokio::sync::Mutex<state::turn::TurnState>> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:546"
    },
    {
      "callee": "<std::sync::Arc<turn_metadata::TurnMetadataState> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:541"
    },
    {
      "callee": "<std::vec::Vec<(&str, &str)> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:566"
    },
    {
      "callee": "<std::vec::Vec<(&str, &str)> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:595"
    },
    {
      "callee": "<std::vec::Vec<(&str, &str)> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:596"
    },
    {
      "callee": "<std::vec::Vec<(&str, &str)> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:687"
    },
    {
      "callee": "<std::vec::Vec<(&str, &str)> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:688"
    },
    {
      "callee": "<std::vec::Vec<codex_protocol::parse_command::ParsedCommand> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:666"
    },
    {
      "callee": "<tokio::sync::MutexGuard<'_, state::turn::TurnState> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:547"
    },
    {
      "callee": "core::fmt::rt::Argument::<'_>::new_display::<&codex_protocol::ToolName>",
      "category": "declaration",
      "def_path_hash": "f912a25b9b2af1492bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:856"
    },
    {
      "callee": "core::fmt::rt::Argument::<'_>::new_display::<codex_protocol::ToolName>",
      "category": "declaration",
      "def_path_hash": "f912a25b9b2af1492bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:586 (macro)"
    },
    {
      "callee": "tokio::sync::Mutex::<state::turn::TurnState>::lock",
      "category": "declaration",
      "def_path_hash": "fbc7021946db62c1714909b4a5023950",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:546"
    },
    {
      "callee": "tokio::sync::Mutex::<std::option::Option<state::turn::ActiveTurn>>::lock",
      "category": "declaration",
      "def_path_hash": "fbc7021946db62c1714909b4a5023950",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/registry.rs:544"
    },
    {
      "callee": "std::time::SystemTime::now",
      "category": "declaration",
      "def_path_hash": "ffeb66a44abbd8e87e6be08242084ac8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "analytics/src/lib.rs:98"
    }
  ]
}
```
