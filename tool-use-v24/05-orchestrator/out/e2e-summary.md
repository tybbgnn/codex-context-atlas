# 验收结果

passed

MIR：通过，但有 11 项缺 MIR

全部必需检查已通过，主 body BB 全覆盖。公开报告省略本机命令与日志路径。

```json
{
  "status": "passed",
  "passed": true,
  "clean_pass": false,
  "mir_status": "通过，但有 11 项缺 MIR",
  "missing_mir_count": 11,
  "counts": {
    "action_count": 24,
    "bb_covered": 694,
    "bb_total": 694,
    "execution_node_count": 73,
    "goal_count": 8,
    "message_count": 78,
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
      "callee": "<std::result::Result<tools::orchestrator::OrchestratorRunResult<Out>, tools::sandboxing::ToolError> as std::ops::FromResidual<std::result::Result<std::convert::Infallible, tools::sandboxing::ToolError>>>::from_residual",
      "category": "declaration",
      "def_path_hash": "006f519113f498ad2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:167 (macro)"
    },
    {
      "callee": "<std::result::Result<tools::orchestrator::OrchestratorRunResult<Out>, tools::sandboxing::ToolError> as std::ops::FromResidual<std::result::Result<std::convert::Infallible, tools::sandboxing::ToolError>>>::from_residual",
      "category": "declaration",
      "def_path_hash": "006f519113f498ad2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:182 (macro)"
    },
    {
      "callee": "<std::result::Result<tools::orchestrator::OrchestratorRunResult<Out>, tools::sandboxing::ToolError> as std::ops::FromResidual<std::result::Result<std::convert::Infallible, tools::sandboxing::ToolError>>>::from_residual",
      "category": "declaration",
      "def_path_hash": "006f519113f498ad2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:200 (macro)"
    },
    {
      "callee": "<std::result::Result<tools::orchestrator::OrchestratorRunResult<Out>, tools::sandboxing::ToolError> as std::ops::FromResidual<std::result::Result<std::convert::Infallible, tools::sandboxing::ToolError>>>::from_residual",
      "category": "declaration",
      "def_path_hash": "006f519113f498ad2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:215 (macro)"
    },
    {
      "callee": "<std::result::Result<tools::orchestrator::OrchestratorRunResult<Out>, tools::sandboxing::ToolError> as std::ops::FromResidual<std::result::Result<std::convert::Infallible, tools::sandboxing::ToolError>>>::from_residual",
      "category": "declaration",
      "def_path_hash": "006f519113f498ad2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:428 (macro)"
    },
    {
      "callee": "<std::result::Result<tools::orchestrator::OrchestratorRunResult<Out>, tools::sandboxing::ToolError> as std::ops::FromResidual<std::result::Result<std::convert::Infallible, tools::sandboxing::ToolError>>>::from_residual",
      "category": "declaration",
      "def_path_hash": "006f519113f498ad2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:444 (macro)"
    },
    {
      "callee": "<tracing::Level as std::cmp::PartialOrd<tracing::level_filters::LevelFilter>>::le",
      "category": "declaration",
      "def_path_hash": "05ddace4dddbaf572bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:2807"
    },
    {
      "callee": "tracing::Metadata::<'_>::fields",
      "category": "declaration",
      "def_path_hash": "0a622101c76a53bb5f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:914"
    },
    {
      "callee": "core::panicking::panic_fmt",
      "category": "declaration",
      "def_path_hash": "0d96ec32223158742bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.rustup/toolchains/nightly-2026-03-01-aarch64-apple-darwin/lib/rustlib/src/rust/library/core/src/panic.rs:62"
    },
    {
      "callee": "std::option::Option::<&codex_network_proxy::EnvironmentNetworkPolicy>::is_some_and::<{closure@core/src/tools/orchestrator.rs:250:34: 250:42}>",
      "category": "declaration",
      "def_path_hash": "129c332e6ae6760d2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:247"
    },
    {
      "callee": "std::option::Option::<&config::network_proxy_spec::NetworkProxySpec>::is_some_and::<for<'a> fn(&'a config::network_proxy_spec::NetworkProxySpec) -> bool {config::network_proxy_spec::NetworkProxySpec::enabled}>",
      "category": "declaration",
      "def_path_hash": "129c332e6ae6760d2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:241"
    },
    {
      "callee": "tracing::__macro_support::__is_enabled",
      "category": "declaration",
      "def_path_hash": "181afd5c325c6bab417ad177881c8bc3",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:899"
    },
    {
      "callee": "std::fmt::Arguments::<'_>::from_str_nonconst",
      "category": "declaration",
      "def_path_hash": "19819a7ed67a09972bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.rustup/toolchains/nightly-2026-03-01-aarch64-apple-darwin/lib/rustlib/src/rust/library/core/src/panic.rs:62"
    },
    {
      "callee": "<str as std::string::ToString>::to_string",
      "category": "declaration",
      "def_path_hash": "227cbef13c3894950881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:555"
    },
    {
      "callee": "<T as tools::sandboxing::ToolRuntime<Rq, Out>>::turn_environment",
      "category": "out-of-scope",
      "def_path_hash": "25f41320933dd6827f347cbdcc2b778a",
      "reason": "definition exists but extraction container has no body (body_available=False)",
      "rerun_command": "python3 \"$MIRLOADER_ROOT/mirloader.py\" --definitions '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/posts/codex-context/v3/v3-1-2-claude/03outputs/definitions/definitions.json' --scope \"$MIR_SCOPE_WITH_MISSING_DEFINITIONS\" --workspace '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/codex/codex-rs' --output-dir \"$MIR_REEXTRACT_OUTPUT\" --result-file \"$MIR_REEXTRACT_OUTPUT/mir-bodies.json\" --offline --jobs 8",
      "scope_requirement": "Generate a scope-definitions JSON including <T as tools::sandboxing::ToolRuntime<Rq, Out>>::turn_environment (25f41320933dd6827f347cbdcc2b778a); --scope accepts a scope file, not a callee name.",
      "source_line": "core/src/tools/orchestrator.rs:140",
      "tool_reference": "$HOME/ai/codex拆解/v3/v3-1-2-claude/02scrpits/03-mir-extraction/mirloader/README.md"
    },
    {
      "callee": "<T as tools::sandboxing::Sandboxable>::sandbox_preference",
      "category": "out-of-scope",
      "def_path_hash": "264e1434024634fa7f347cbdcc2b778a",
      "reason": "definition exists but extraction container has no body (body_available=False)",
      "rerun_command": "python3 \"$MIRLOADER_ROOT/mirloader.py\" --definitions '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/posts/codex-context/v3/v3-1-2-claude/03outputs/definitions/definitions.json' --scope \"$MIR_SCOPE_WITH_MISSING_DEFINITIONS\" --workspace '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/codex/codex-rs' --output-dir \"$MIR_REEXTRACT_OUTPUT\" --result-file \"$MIR_REEXTRACT_OUTPUT/mir-bodies.json\" --offline --jobs 8",
      "scope_requirement": "Generate a scope-definitions JSON including <T as tools::sandboxing::Sandboxable>::sandbox_preference (264e1434024634fa7f347cbdcc2b778a); --scope accepts a scope file, not a callee name.",
      "source_line": "core/src/tools/orchestrator.rs:265",
      "tool_reference": "$HOME/ai/codex拆解/v3/v3-1-2-claude/02scrpits/03-mir-extraction/mirloader/README.md"
    },
    {
      "callee": "tracing::subscriber::Interest::is_never",
      "category": "declaration",
      "def_path_hash": "266ce036cd642c235f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:899"
    },
    {
      "callee": "codex_sandboxing::policy_transforms::effective_network_sandbox_policy",
      "category": "out-of-scope",
      "def_path_hash": "2857c692c16fa349ab9aa54c4ae74daa",
      "reason": "definition exists but extraction container has no body (body_available=True)",
      "rerun_command": "python3 \"$MIRLOADER_ROOT/mirloader.py\" --definitions '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/posts/codex-context/v3/v3-1-2-claude/03outputs/definitions/definitions.json' --scope \"$MIR_SCOPE_WITH_MISSING_DEFINITIONS\" --workspace '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/codex/codex-rs' --output-dir \"$MIR_REEXTRACT_OUTPUT\" --result-file \"$MIR_REEXTRACT_OUTPUT/mir-bodies.json\" --offline --jobs 8",
      "scope_requirement": "Generate a scope-definitions JSON including codex_sandboxing::policy_transforms::effective_network_sandbox_policy (2857c692c16fa349ab9aa54c4ae74daa); --scope accepts a scope file, not a callee name.",
      "source_line": "core/src/tools/orchestrator.rs:255",
      "tool_reference": "$HOME/ai/codex拆解/v3/v3-1-2-claude/02scrpits/03-mir-extraction/mirloader/README.md"
    },
    {
      "callee": "tracing::level_filters::LevelFilter::current",
      "category": "declaration",
      "def_path_hash": "2cc74db53adc0c125f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:2808"
    },
    {
      "callee": "<std::boxed::Box<codex_protocol::exec_output::ExecToolCallOutput> as std::convert::AsRef<codex_protocol::exec_output::ExecToolCallOutput>>::as_ref",
      "category": "declaration",
      "def_path_hash": "39d972858970f2b32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:414"
    },
    {
      "callee": "<std::sync::Arc<session::turn_context::TurnContext> as std::convert::AsRef<session::turn_context::TurnContext>>::as_ref",
      "category": "declaration",
      "def_path_hash": "39d972858970f2b32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:131"
    },
    {
      "callee": "<impl FnOnce(FileSystemSandboxPolicy) -> FileSystemSandboxPolicy as std::ops::FnOnce<(permissions::FileSystemSandboxPolicy,)>>::call_once",
      "category": "declaration",
      "def_path_hash": "474678101bb128de2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "protocol/src/models.rs:598"
    },
    {
      "callee": "std::pin::Pin::<&mut {async fn body of session::<impl session::session::Session>::strict_auto_review_enabled()}>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:136 (macro)"
    },
    {
      "callee": "std::pin::Pin::<&mut {async fn body of tools::approvals::<impl session::session::Session>::request_approval()}>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:185 (macro)"
    },
    {
      "callee": "std::pin::Pin::<&mut {async fn body of tools::approvals::<impl session::session::Session>::request_approval()}>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:218 (macro)"
    },
    {
      "callee": "std::pin::Pin::<&mut {async fn body of tools::approvals::<impl session::session::Session>::request_approval()}>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:447 (macro)"
    },
    {
      "callee": "std::pin::Pin::<&mut {async fn body of tools::orchestrator::ToolOrchestrator::run_attempt<Rq, Out, T>()}>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:317 (macro)"
    },
    {
      "callee": "std::pin::Pin::<&mut {async fn body of tools::orchestrator::ToolOrchestrator::run_attempt<Rq, Out, T>()}>::new_unchecked",
      "category": "declaration",
      "def_path_hash": "57dad189d36364332bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:494 (macro)"
    },
    {
      "callee": "<{async fn body of session::<impl session::session::Session>::strict_auto_review_enabled()} as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:136 (macro)"
    },
    {
      "callee": "<{async fn body of tools::approvals::<impl session::session::Session>::request_approval()} as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:185 (macro)"
    },
    {
      "callee": "<{async fn body of tools::approvals::<impl session::session::Session>::request_approval()} as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:218 (macro)"
    },
    {
      "callee": "<{async fn body of tools::approvals::<impl session::session::Session>::request_approval()} as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:447 (macro)"
    },
    {
      "callee": "<{async fn body of tools::orchestrator::ToolOrchestrator::run_attempt<Rq, Out, T>()} as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:317 (macro)"
    },
    {
      "callee": "<{async fn body of tools::orchestrator::ToolOrchestrator::run_attempt<Rq, Out, T>()} as futures::Future>::poll",
      "category": "declaration",
      "def_path_hash": "591fc3e935af0c362bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:494 (macro)"
    },
    {
      "callee": "codex_sandboxing::SandboxManager::should_sandbox",
      "category": "out-of-scope",
      "def_path_hash": "592a0297eeab7c90ab9aa54c4ae74daa",
      "reason": "definition exists but extraction container has no body (body_available=True)",
      "rerun_command": "python3 \"$MIRLOADER_ROOT/mirloader.py\" --definitions '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/posts/codex-context/v3/v3-1-2-claude/03outputs/definitions/definitions.json' --scope \"$MIR_SCOPE_WITH_MISSING_DEFINITIONS\" --workspace '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/codex/codex-rs' --output-dir \"$MIR_REEXTRACT_OUTPUT\" --result-file \"$MIR_REEXTRACT_OUTPUT/mir-bodies.json\" --offline --jobs 8",
      "scope_requirement": "Generate a scope-definitions JSON including codex_sandboxing::SandboxManager::should_sandbox (592a0297eeab7c90ab9aa54c4ae74daa); --scope accepts a scope file, not a callee name.",
      "source_line": "core/src/tools/orchestrator.rs:268",
      "tool_reference": "$HOME/ai/codex拆解/v3/v3-1-2-claude/02scrpits/03-mir-extraction/mirloader/README.md"
    },
    {
      "callee": "std::option::Option::<codex_protocol::approvals::NetworkApprovalContext>::is_none",
      "category": "declaration",
      "def_path_hash": "5d286d68af91d5e62bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:352"
    },
    {
      "callee": "std::option::Option::<codex_protocol::approvals::NetworkApprovalContext>::is_none",
      "category": "declaration",
      "def_path_hash": "5d286d68af91d5e62bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:397"
    },
    {
      "callee": "std::option::Option::<codex_protocol::approvals::NetworkApprovalContext>::is_none",
      "category": "declaration",
      "def_path_hash": "5d286d68af91d5e62bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:421"
    },
    {
      "callee": "tracing::callsite::DefaultCallsite::interest",
      "category": "declaration",
      "def_path_hash": "6141864431f3336c5f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:898"
    },
    {
      "callee": "codex_sandboxing::SandboxManager::new",
      "category": "out-of-scope",
      "def_path_hash": "631282f4a4bba4c3ab9aa54c4ae74daa",
      "reason": "definition exists but extraction container has no body (body_available=True)",
      "rerun_command": "python3 \"$MIRLOADER_ROOT/mirloader.py\" --definitions '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/posts/codex-context/v3/v3-1-2-claude/03outputs/definitions/definitions.json' --scope \"$MIR_SCOPE_WITH_MISSING_DEFINITIONS\" --workspace '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/codex/codex-rs' --output-dir \"$MIR_REEXTRACT_OUTPUT\" --result-file \"$MIR_REEXTRACT_OUTPUT/mir-bodies.json\" --offline --jobs 8",
      "scope_requirement": "Generate a scope-definitions JSON including codex_sandboxing::SandboxManager::new (631282f4a4bba4c3ab9aa54c4ae74daa); --scope accepts a scope file, not a callee name.",
      "source_line": "core/src/tools/orchestrator.rs:141",
      "tool_reference": "$HOME/ai/codex拆解/v3/v3-1-2-claude/02scrpits/03-mir-extraction/mirloader/README.md"
    },
    {
      "callee": "std::fmt::Arguments::<'_>::new::<38, 1>",
      "category": "declaration",
      "def_path_hash": "6488302cb95ba4ee2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.rustup/toolchains/nightly-2026-03-01-aarch64-apple-darwin/lib/rustlib/src/rust/library/alloc/src/macros.rs:114"
    },
    {
      "callee": "std::fmt::Arguments::<'_>::new::<46, 1>",
      "category": "declaration",
      "def_path_hash": "6488302cb95ba4ee2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.rustup/toolchains/nightly-2026-03-01-aarch64-apple-darwin/lib/rustlib/src/rust/library/alloc/src/macros.rs:114 (macro)"
    },
    {
      "callee": "std::option::Option::<codex_network_proxy::EnvironmentNetworkPolicy>::is_some",
      "category": "declaration",
      "def_path_hash": "6a48af0263ed1c4a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:150"
    },
    {
      "callee": "std::option::Option::<codex_network_proxy::NetworkProxy>::is_some",
      "category": "declaration",
      "def_path_hash": "6a48af0263ed1c4a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:263"
    },
    {
      "callee": "std::option::Option::<codex_protocol::approvals::NetworkApprovalContext>::is_some",
      "category": "declaration",
      "def_path_hash": "6a48af0263ed1c4a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:378"
    },
    {
      "callee": "std::option::Option::<codex_protocol::network_policy::NetworkPolicyDecisionPayload>::is_some",
      "category": "declaration",
      "def_path_hash": "6a48af0263ed1c4a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:352"
    },
    {
      "callee": "std::option::Option::<tools::network_approval::NetworkApprovalSpec>::is_some",
      "category": "declaration",
      "def_path_hash": "6a48af0263ed1c4a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:251"
    },
    {
      "callee": "std::vec::Vec::<permissions::FileSystemSandboxEntry>::new",
      "category": "declaration",
      "def_path_hash": "70abb47554dd12f50881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "protocol/src/permissions.rs:630"
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
      "callee": "std::option::Option::<codex_utils_path_uri::PathUri>::unwrap_or_else::<{closure@core/src/tools/orchestrator.rs:292:29: 292:31}>",
      "category": "declaration",
      "def_path_hash": "7c70afa9f20534cc2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:289"
    },
    {
      "callee": "std::option::Option::<tools::sandboxing::ExecApprovalRequirement>::unwrap_or_else::<{closure@core/src/tools/orchestrator.rs:161:78: 161:80}>",
      "category": "declaration",
      "def_path_hash": "7c70afa9f20534cc2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:161"
    },
    {
      "callee": "<tracing::callsite::DefaultCallsite as tracing::Callsite>::metadata",
      "category": "declaration",
      "def_path_hash": "8134ffbf34a2a9aa5f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:899"
    },
    {
      "callee": "codex_sandboxing::SandboxManager::with_allowed_symlinked_codex_home",
      "category": "out-of-scope",
      "def_path_hash": "91f3f5ff54c0d610ab9aa54c4ae74daa",
      "reason": "definition exists but extraction container has no body (body_available=True)",
      "rerun_command": "python3 \"$MIRLOADER_ROOT/mirloader.py\" --definitions '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/posts/codex-context/v3/v3-1-2-claude/03outputs/definitions/definitions.json' --scope \"$MIR_SCOPE_WITH_MISSING_DEFINITIONS\" --workspace '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/codex/codex-rs' --output-dir \"$MIR_REEXTRACT_OUTPUT\" --result-file \"$MIR_REEXTRACT_OUTPUT/mir-bodies.json\" --offline --jobs 8",
      "scope_requirement": "Generate a scope-definitions JSON including codex_sandboxing::SandboxManager::with_allowed_symlinked_codex_home (91f3f5ff54c0d610ab9aa54c4ae74daa); --scope accepts a scope file, not a callee name.",
      "source_line": "core/src/tools/orchestrator.rs:143",
      "tool_reference": "$HOME/ai/codex拆解/v3/v3-1-2-claude/02scrpits/03-mir-extraction/mirloader/README.md"
    },
    {
      "callee": "codex_protocol::sandbox::effective_windows_sandbox_type",
      "category": "out-of-scope",
      "def_path_hash": "949fc1a7ba15a794fd9ac5127673ba6d",
      "reason": "definition exists but extraction container has no body (body_available=True)",
      "rerun_command": "python3 \"$MIRLOADER_ROOT/mirloader.py\" --definitions '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/posts/codex-context/v3/v3-1-2-claude/03outputs/definitions/definitions.json' --scope \"$MIR_SCOPE_WITH_MISSING_DEFINITIONS\" --workspace '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/codex/codex-rs' --output-dir \"$MIR_REEXTRACT_OUTPUT\" --result-file \"$MIR_REEXTRACT_OUTPUT/mir-bodies.json\" --offline --jobs 8",
      "scope_requirement": "Generate a scope-definitions JSON including codex_protocol::sandbox::effective_windows_sandbox_type (949fc1a7ba15a794fd9ac5127673ba6d); --scope accepts a scope file, not a callee name.",
      "source_line": "core/src/tools/orchestrator.rs:274",
      "tool_reference": "$HOME/ai/codex拆解/v3/v3-1-2-claude/02scrpits/03-mir-extraction/mirloader/README.md"
    },
    {
      "callee": "std::borrow::Cow::<'_, str>::into_owned",
      "category": "declaration",
      "def_path_hash": "99deabefc370f0d10881b6f26f9b543c",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:134"
    },
    {
      "callee": "<codex_utils_path_uri::PathUri as std::clone::Clone>::clone",
      "category": "out-of-scope",
      "def_path_hash": "a06578f871e6014046072e0d4ac9267f",
      "reason": "definition exists but extraction container has no body (body_available=True)",
      "rerun_command": "python3 \"$MIRLOADER_ROOT/mirloader.py\" --definitions '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/posts/codex-context/v3/v3-1-2-claude/03outputs/definitions/definitions.json' --scope \"$MIR_SCOPE_WITH_MISSING_DEFINITIONS\" --workspace '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/codex/codex-rs' --output-dir \"$MIR_REEXTRACT_OUTPUT\" --result-file \"$MIR_REEXTRACT_OUTPUT/mir-bodies.json\" --offline --jobs 8",
      "scope_requirement": "Generate a scope-definitions JSON including <codex_utils_path_uri::PathUri as std::clone::Clone>::clone (a06578f871e6014046072e0d4ac9267f); --scope accepts a scope file, not a callee name.",
      "source_line": "core/src/tools/orchestrator.rs:292",
      "tool_reference": "$HOME/ai/codex拆解/v3/v3-1-2-claude/02scrpits/03-mir-extraction/mirloader/README.md"
    },
    {
      "callee": "std::option::Option::<codex_network_proxy::EnvironmentNetworkPolicy>::as_ref",
      "category": "declaration",
      "def_path_hash": "a11824a548d0e6b32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:247"
    },
    {
      "callee": "std::option::Option::<codex_protocol::approvals::NetworkApprovalContext>::as_ref",
      "category": "declaration",
      "def_path_hash": "a11824a548d0e6b32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:408"
    },
    {
      "callee": "std::option::Option::<codex_protocol::network_policy::NetworkPolicyDecisionPayload>::as_ref",
      "category": "declaration",
      "def_path_hash": "a11824a548d0e6b32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:346"
    },
    {
      "callee": "std::option::Option::<config::network_proxy_spec::NetworkProxySpec>::as_ref",
      "category": "declaration",
      "def_path_hash": "a11824a548d0e6b32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:241"
    },
    {
      "callee": "std::option::Option::<runtime_options::ExecServerRuntimeOptions>::as_ref",
      "category": "declaration",
      "def_path_hash": "a11824a548d0e6b32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "exec-server/src/environment.rs:894"
    },
    {
      "callee": "std::option::Option::<std::path::PathBuf>::as_ref",
      "category": "declaration",
      "def_path_hash": "a11824a548d0e6b32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:294"
    },
    {
      "callee": "std::option::Option::<std::path::PathBuf>::as_ref",
      "category": "declaration",
      "def_path_hash": "a11824a548d0e6b32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:296"
    },
    {
      "callee": "std::option::Option::<tools::network_approval::NetworkApprovalSpec>::as_ref",
      "category": "declaration",
      "def_path_hash": "a11824a548d0e6b32bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:257"
    },
    {
      "callee": "std::time::Duration::as_millis",
      "category": "declaration",
      "def_path_hash": "ad8fc1ab54f15df62bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "otel/src/events/session_telemetry.rs:1203"
    },
    {
      "callee": "<guardian::GuardianReviewContext as std::convert::From<&std::sync::Arc<session::step_context::StepContext>>>::from",
      "category": "declaration",
      "def_path_hash": "b1505aa240e0ea7c2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:173"
    },
    {
      "callee": "<guardian::GuardianReviewContext as std::convert::From<&std::sync::Arc<session::step_context::StepContext>>>::from",
      "category": "declaration",
      "def_path_hash": "b1505aa240e0ea7c2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:206"
    },
    {
      "callee": "<guardian::GuardianReviewContext as std::convert::From<&std::sync::Arc<session::step_context::StepContext>>>::from",
      "category": "declaration",
      "def_path_hash": "b1505aa240e0ea7c2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:434"
    },
    {
      "callee": "std::result::Result::<tools::approvals::ApprovalAction, std::io::Error>::map_err::<tools::sandboxing::ToolError, {closure@core/src/tools/orchestrator.rs:169:34: 169:39}>",
      "category": "declaration",
      "def_path_hash": "b208b59e6d19ae672bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:167"
    },
    {
      "callee": "std::result::Result::<tools::approvals::ApprovalAction, std::io::Error>::map_err::<tools::sandboxing::ToolError, {closure@core/src/tools/orchestrator.rs:202:30: 202:35}>",
      "category": "declaration",
      "def_path_hash": "b208b59e6d19ae672bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:200"
    },
    {
      "callee": "std::result::Result::<tools::approvals::ApprovalAction, std::io::Error>::map_err::<tools::sandboxing::ToolError, {closure@core/src/tools/orchestrator.rs:430:34: 430:39}>",
      "category": "declaration",
      "def_path_hash": "b208b59e6d19ae672bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:428"
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
      "callee": "events::shared::tool_namespace",
      "category": "out-of-scope",
      "def_path_hash": "b797943e48228e06b2ef0825835d5d2b",
      "reason": "definition exists but extraction container has no body (body_available=True)",
      "rerun_command": "python3 \"$MIRLOADER_ROOT/mirloader.py\" --definitions '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/posts/codex-context/v3/v3-1-2-claude/03outputs/definitions/definitions.json' --scope \"$MIR_SCOPE_WITH_MISSING_DEFINITIONS\" --workspace '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/codex/codex-rs' --output-dir \"$MIR_REEXTRACT_OUTPUT\" --result-file \"$MIR_REEXTRACT_OUTPUT/mir-bodies.json\" --offline --jobs 8",
      "scope_requirement": "Generate a scope-definitions JSON including events::shared::tool_namespace (b797943e48228e06b2ef0825835d5d2b); --scope accepts a scope file, not a callee name.",
      "source_line": "otel/src/events/session_telemetry.rs:1173",
      "tool_reference": "$HOME/ai/codex拆解/v3/v3-1-2-claude/02scrpits/03-mir-extraction/mirloader/README.md"
    },
    {
      "callee": "tracing::field::display::<&std::string::String>",
      "category": "declaration",
      "def_path_hash": "b9118929da094bd45f065356c969b0a0",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "../../../../../../../../../../.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/tracing-0.1.44/src/macros.rs:2836"
    },
    {
      "callee": "codex_sandboxing::SandboxManager::select_initial",
      "category": "out-of-scope",
      "def_path_hash": "b954d3439812dbe2ab9aa54c4ae74daa",
      "reason": "definition exists but extraction container has no body (body_available=True)",
      "rerun_command": "python3 \"$MIRLOADER_ROOT/mirloader.py\" --definitions '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/posts/codex-context/v3/v3-1-2-claude/03outputs/definitions/definitions.json' --scope \"$MIR_SCOPE_WITH_MISSING_DEFINITIONS\" --workspace '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/codex/codex-rs' --output-dir \"$MIR_REEXTRACT_OUTPUT\" --result-file \"$MIR_REEXTRACT_OUTPUT/mir-bodies.json\" --offline --jobs 8",
      "scope_requirement": "Generate a scope-definitions JSON including codex_sandboxing::SandboxManager::select_initial (b954d3439812dbe2ab9aa54c4ae74daa); --scope accepts a scope file, not a callee name.",
      "source_line": "core/src/tools/orchestrator.rs:279",
      "tool_reference": "$HOME/ai/codex拆解/v3/v3-1-2-claude/02scrpits/03-mir-extraction/mirloader/README.md"
    },
    {
      "callee": "std::time::Instant::elapsed",
      "category": "declaration",
      "def_path_hash": "c3dabd15f461f5e07e6be08242084ac8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:318"
    },
    {
      "callee": "std::time::Instant::elapsed",
      "category": "declaration",
      "def_path_hash": "c3dabd15f461f5e07e6be08242084ac8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:495"
    },
    {
      "callee": "<std::result::Result<codex_protocol::protocol::ReviewDecision, tools::sandboxing::ToolError> as std::ops::Try>::branch",
      "category": "declaration",
      "def_path_hash": "c554288a6d26ad412bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:182 (macro)"
    },
    {
      "callee": "<std::result::Result<codex_protocol::protocol::ReviewDecision, tools::sandboxing::ToolError> as std::ops::Try>::branch",
      "category": "declaration",
      "def_path_hash": "c554288a6d26ad412bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:215 (macro)"
    },
    {
      "callee": "<std::result::Result<codex_protocol::protocol::ReviewDecision, tools::sandboxing::ToolError> as std::ops::Try>::branch",
      "category": "declaration",
      "def_path_hash": "c554288a6d26ad412bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:444 (macro)"
    },
    {
      "callee": "<std::result::Result<tools::approvals::ApprovalAction, tools::sandboxing::ToolError> as std::ops::Try>::branch",
      "category": "declaration",
      "def_path_hash": "c554288a6d26ad412bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:167 (macro)"
    },
    {
      "callee": "<std::result::Result<tools::approvals::ApprovalAction, tools::sandboxing::ToolError> as std::ops::Try>::branch",
      "category": "declaration",
      "def_path_hash": "c554288a6d26ad412bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:200 (macro)"
    },
    {
      "callee": "<std::result::Result<tools::approvals::ApprovalAction, tools::sandboxing::ToolError> as std::ops::Try>::branch",
      "category": "declaration",
      "def_path_hash": "c554288a6d26ad412bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:428 (macro)"
    },
    {
      "callee": "std::time::Instant::now",
      "category": "declaration",
      "def_path_hash": "c9a699096f0df9507e6be08242084ac8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:315"
    },
    {
      "callee": "std::time::Instant::now",
      "category": "declaration",
      "def_path_hash": "c9a699096f0df9507e6be08242084ac8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:491"
    },
    {
      "callee": "<{async fn body of session::<impl session::session::Session>::strict_auto_review_enabled()} as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:136 (macro)"
    },
    {
      "callee": "<{async fn body of tools::approvals::<impl session::session::Session>::request_approval()} as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:185 (macro)"
    },
    {
      "callee": "<{async fn body of tools::approvals::<impl session::session::Session>::request_approval()} as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:218 (macro)"
    },
    {
      "callee": "<{async fn body of tools::approvals::<impl session::session::Session>::request_approval()} as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:447 (macro)"
    },
    {
      "callee": "<{async fn body of tools::orchestrator::ToolOrchestrator::run_attempt<Rq, Out, T>()} as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:317 (macro)"
    },
    {
      "callee": "<{async fn body of tools::orchestrator::ToolOrchestrator::run_attempt<Rq, Out, T>()} as std::future::IntoFuture>::into_future",
      "category": "declaration",
      "def_path_hash": "d568101b07447f112bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:494 (macro)"
    },
    {
      "callee": "<codex_otel::SessionTelemetry as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:133"
    },
    {
      "callee": "<std::option::Option<codex_protocol::approvals::NetworkApprovalContext> as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:441"
    },
    {
      "callee": "<std::option::Option<std::string::String> as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:211"
    },
    {
      "callee": "<std::option::Option<std::string::String> as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:424"
    },
    {
      "callee": "<std::string::String as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:175"
    },
    {
      "callee": "<std::string::String as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:197"
    },
    {
      "callee": "<std::string::String as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:208"
    },
    {
      "callee": "<std::string::String as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:436"
    },
    {
      "callee": "<tokio_util::sync::CancellationToken as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:174"
    },
    {
      "callee": "<tokio_util::sync::CancellationToken as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:207"
    },
    {
      "callee": "<tokio_util::sync::CancellationToken as std::clone::Clone>::clone",
      "category": "declaration",
      "def_path_hash": "e0eda86b01817d1a2bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:435"
    },
    {
      "callee": "<T as tools::sandboxing::Approvable<Rq>>::approval_action",
      "category": "out-of-scope",
      "def_path_hash": "e45ccfb8f94fdc5a7f347cbdcc2b778a",
      "reason": "definition exists but extraction container has no body (body_available=False)",
      "rerun_command": "python3 \"$MIRLOADER_ROOT/mirloader.py\" --definitions '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/posts/codex-context/v3/v3-1-2-claude/03outputs/definitions/definitions.json' --scope \"$MIR_SCOPE_WITH_MISSING_DEFINITIONS\" --workspace '$HOME/Library/Mobile Documents/iCloud~md~obsidian/Documents/ai product hunter/pm2builder/6-posts/codex-文科生真的看懂harness/codex/codex-rs' --output-dir \"$MIR_REEXTRACT_OUTPUT\" --result-file \"$MIR_REEXTRACT_OUTPUT/mir-bodies.json\" --offline --jobs 8",
      "scope_requirement": "Generate a scope-definitions JSON including <T as tools::sandboxing::Approvable<Rq>>::approval_action (e45ccfb8f94fdc5a7f347cbdcc2b778a); --scope accepts a scope file, not a callee name.",
      "source_line": "core/src/tools/orchestrator.rs:167",
      "tool_reference": "$HOME/ai/codex拆解/v3/v3-1-2-claude/02scrpits/03-mir-extraction/mirloader/README.md"
    },
    {
      "callee": "std::option::Option::<&codex_exec_server::ExecServerRuntimeOptions>::and_then::<codex_utils_absolute_path::AbsolutePathBuf, {closure@core/src/tools/orchestrator.rs:147:27: 147:34}>",
      "category": "declaration",
      "def_path_hash": "eb7d8a851e1450322bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:144"
    },
    {
      "callee": "std::option::Option::<&codex_protocol::network_policy::NetworkPolicyDecisionPayload>::and_then::<codex_protocol::approvals::NetworkApprovalContext, for<'a> fn(&'a codex_protocol::network_policy::NetworkPolicyDecisionPayload) -> std::option::Option<codex_protocol::approvals::NetworkApprovalContext> {network_policy_decision::network_approval_context_from_payload}>",
      "category": "declaration",
      "def_path_hash": "eb7d8a851e1450322bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:346"
    },
    {
      "callee": "std::option::Option::<&tools::network_approval::NetworkApprovalSpec>::and_then::<&codex_protocol::models::AdditionalPermissionProfile, {closure@core/src/tools/orchestrator.rs:259:39: 259:45}>",
      "category": "declaration",
      "def_path_hash": "eb7d8a851e1450322bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:257"
    },
    {
      "callee": "std::option::Option::<usize>::and_then::<std::num::NonZero<usize>, fn(usize) -> std::option::Option<std::num::NonZero<usize>> {std::num::NonZero::<usize>::new}>",
      "category": "declaration",
      "def_path_hash": "eb7d8a851e1450322bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "protocol/src/models.rs:383"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:168"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:190"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:201"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:336"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:337"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:354"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:355"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:364"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:365"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:388"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:389"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:399"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:400"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:429"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:499"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:500"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:513"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:514"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:527"
    },
    {
      "callee": "<std::string::String as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:528"
    },
    {
      "callee": "<std::sync::Arc<codex_exec_server::Environment> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:144"
    },
    {
      "callee": "<std::sync::Arc<config::Config> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:241"
    },
    {
      "callee": "<std::sync::Arc<config::Config> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:294"
    },
    {
      "callee": "<std::sync::Arc<config::Config> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:296"
    },
    {
      "callee": "<std::sync::Arc<session::session::Session> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:136"
    },
    {
      "callee": "<std::sync::Arc<session::step_context::StepContext> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:131"
    },
    {
      "callee": "<std::sync::Arc<session::step_context::StepContext> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:132"
    },
    {
      "callee": "<std::sync::Arc<session::step_settings::ResolvedStepSettings> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:132"
    },
    {
      "callee": "<std::sync::Arc<session::step_settings::StepSettings> as std::ops::Deref>::deref",
      "category": "declaration",
      "def_path_hash": "edf7108b995e0d952bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/session/step_settings.rs:100"
    },
    {
      "callee": "std::option::Option::<std::num::NonZero<usize>>::map::<usize, fn(std::num::NonZero<usize>) -> usize {<usize as std::convert::From<std::num::NonZero<usize>>>::from}>",
      "category": "declaration",
      "def_path_hash": "efc1704abda0d2442bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "protocol/src/models.rs:401"
    },
    {
      "callee": "std::option::Option::<&codex_utils_path_uri::PathUri>::cloned",
      "category": "declaration",
      "def_path_hash": "f6f49d8c718620a92bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:289"
    },
    {
      "callee": "core::fmt::rt::Argument::<'_>::new_display::<std::io::Error>",
      "category": "declaration",
      "def_path_hash": "f912a25b9b2af1492bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:431"
    },
    {
      "callee": "core::fmt::rt::Argument::<'_>::new_display::<std::string::String>",
      "category": "declaration",
      "def_path_hash": "f912a25b9b2af1492bac9d628bdc1eb8",
      "reason": "std/third-party declaration absent from definitions",
      "source_line": "core/src/tools/orchestrator.rs:410 (macro)"
    }
  ]
}
```
